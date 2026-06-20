# Regression Suite

## Critical Flow

Employee Salary
→ Payroll Calculation
→ Payslip Generation
→ Employee View

---

### Test Case 1

Update employee salary.

Expected:
New salary appears in next payslip.

---

### Test Case 2

Create new employee.

Expected:
Payroll record generated correctly.

---

### Test Case 3

Employee without salary record.

Expected:
Validation error shown.

---

### Test Case 4

Change salary twice in same period.

Expected:
Latest approved salary used.

---

### Test Case 5

Generate payslip after salary update.

Expected:
Correct amount displayed.

---

## Dependency Testing

### Attendance → Payroll

Update attendance.

Expected:
Payroll recalculated.

---

### Leave → Payroll

Approve leave.

Expected:
Payroll updated.

---

### Overtime → Payroll

Add overtime.

Expected:
Salary updated correctly.
