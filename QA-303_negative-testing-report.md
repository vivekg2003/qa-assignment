# Negative Testing Audit

## Objective

Verify application behavior against invalid and malicious inputs.

---

## Empty Input Testing

### Test

Submit empty forms.

Expected:
Validation messages displayed.

---

## Boundary Testing

Tested Values:

- 0
- -1
- 999999999

Expected:
Invalid values rejected.

---

## Invalid Data Types

Tested:

- Numbers in name field
- Text in salary field

Expected:
Input validation should prevent submission.

---

## Security Testing

### XSS

Payload:

<script>alert('xss')</script>

Expected:
Input sanitized.

---

### SQL Injection

Payload:

' OR 1=1 --

Expected:
Request rejected.

---

## Result

Application should safely handle invalid and malicious input.
