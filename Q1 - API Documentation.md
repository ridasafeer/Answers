# API Documentation

All responses are provided as JSON objects
The root syntax for each request includes the **HTTP Operation*** used and the **resource**, shown in the **heading for each endpoint**

Employee profile: Commonly used group of parameters in the employee endpoint
- Employee name
- Department name
- Employee salary

## GET api/get_employee/id

Returns the employee profile to client

### Resource URL

``` http://domain.com/api/get_employee ```

### Parameters 

| Parameter | Description |
| ------------- | ------------- |
| id | id in list of employees acting as identifier for specific employee |

## POST api/add_employee

Uses employee profile parameters to populate data in each table accordingly and returns using ```get_employee``` endpoint in combination to client

### Resource URL

``` http://domain.com/api/add_employee ```

### Parameters 

| Parameter | Description |
| ------------- | ------------- |
| employee_name | name of specified emoployee |
| salary | salary of employee |
| department_id | id in list of departments acting as identifier for specific department |

## POST api/add_department

Creates new department and returns the newly created department name and id

### Resource URL

``` http://domain.com/api/add_department ``` 

### Parameters 

| Parameter | Description |
| ------------- | ------------- |
| employee_name | name of specified emoployee |

### Return 

## PUT api/update_salary/id

Updates salary entry for specificed employee and subsequently returns employee profile from ```get_employee``` endpoint

### Resource URL

``` http://domain.com/api/update_salary ```

### Parameters

| Parameter | Description |
| ------------- | ------------- |
| id | id in list of employees acting as identifier for specific employee |
| new_salary | updated salary for specified employee, updates employee profile |

## DELETE api/terminate_employee

Deletes specified employee and corresponding salary entities from database

### Resource URL

``` http://domain.com/api/terminate_employee ```

### Parameters 

| Parameter | Description |
| ------------- | ------------- |
| id | id in list of employees acting as identifier for specific employee |
