
```json
{
    "firstName": "Turii",
    "lastName": "vindina",
    "jobTitle": "Deve",
    "position": "Senior",
    "role": "Employee",
    "departmentId": ObjectId("5f49ccaa1946f875f207fc56")  // Reference to a department
}
```

**Departments Collection Documents**:
```json
{
    "name": "FCI Department",
    "hodId": ObjectId("5f49ccaa1946f875f207fc57")  // Reference to a user
}
```

**DepartmentObjectives Collection Documents**:
```json
{
    "name": "Improve Customer Satisfaction",
    "weight": 0.8,
    "departmentId": ObjectId("5f49ccaa1946f875f207fc56")  // Reference to a department
}
```

**KPIs Collection Documents**:
```json
{
    "userId": ObjectId("5f49ccaa1946f875f207fc58"),  // Reference to a user
    "name": "Customer Support Tickets Resolved",
    "metric": "Number",
    "unit": "Tickets",
    "score": 92.5
}
```

**ObjectiveKPIRelation Collection Documents**:
```json
{
    "objectiveId": ObjectId("5f49ccaa1946f875f207fc59"),  // Reference to a department objective
    "kpiId": ObjectId("5f49ccaa1946f875f207fc5a")  // Reference to a KPI
}
```

**SupervisorAssignments Collection Documents**:
```json
{
    "supervisorId": ObjectId("5f49ccaa1946f875f207fc57"),  // Reference to a supervisor user
    "employeeId": ObjectId("5f49ccaa1946f875f207fc5b")  // Reference to an employee user
}
```

**SupervisorGrades Collection Documents**:
```json
{
    "supervisorId": ObjectId("5f49ccaa1946f875f207fc57"),  // Reference to a supervisor user
    "kpiId": ObjectId("5f49ccaa1946f875f207fc5a"),  // Reference to a KPI
    "grade": 88.3
}
```

**EmployeeSupervisorFeedback Collection Documents**:
```json
{
    "employeeId": ObjectId("5f49ccaa1946f875f207fc5b"),  
    "supervisorId": ObjectId("5f49ccaa1946f875f207fc57"),  
    "grade": 95.0,
    "feedback": "Excellent performance."
}
```

**UserAuthentication Collection Documents**:
```json
{
    "userId": ObjectId("5f49ccaa1946f875f207fc58"),  // Reference to a user
    "email": "johndoe@example.com",
   
    "salt": "salt_value"
}
```

