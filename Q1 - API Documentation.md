# API Documentation

All responses are provided as JSON objects
Parameters: 

Employee profile: Commonly used group of parameters in the employee endpoint
- Employee name
- Department name
- Employee salary

## GET employees/get_employee/id

Returns the employee profile to client

### Resource URL

``` http://domain.com/api/get_employee ```

### Example Request

## POST employees/add_employee

Uses employee profile parameters to populate data in each table accordingly and returns using ```get_employee``` endpoint in combination to client

### Resource URL

``` http://domain.com/api/add_employee ```

## POST employees/add_department

Creates new department and returns the newly created department name and id

### Resource URL

``` http://domain.com/api/add_department ``` 

## PUT employees/update_salary/id

Updates salary entry for specificed employee and subsequently returns employee profile from ```get_employee``` endpoint

### Resource URL

``` http://domain.com/api/update_salary ```

## DELETE employees/terminate_employee

Deletes specified employee and corresponding salary entities from database

### Resource URL

``` http://domain.com/api/terminate_employee ```
