# HOSPITAL MANAGEMENT SYSTEM
## Aim: 
To create a hospital management system using react, springboot and sql.
## PROGRAM:
```
hospitalmanagement.java
package com.HospitalManagement.hospitalmanagement.patient;
import jakarta.persistence.*;
import org.junit.platform.commons.annotation. Testable;
import org.springframework.boot.autoconfigure.domain.EntityScan;
import java.time.LocalDate;
import java.time.Period;
@Entity
@Table
public class HospitalManagementSystem {
@Id
@SequenceGenerator(
name = "Hospitalmanagement_sequence",
sequenceName = "Hospitalmanagement_sequence", allocationSize = 1
@GeneratedValue(
strategy GenerationType.SEQUENCE,
generator = "Hospitalmanagement_sequence"
private Long PatientId;
Create a job portal application using react,

private String   HospitalmanagementName;
@Transient private Integer PatientAge; private LocalDate PatientDob;
private String patient Email;
public Hospitalmanagement() {}
public hospitalmanagement (Long patientId, String patient Name, LocalDate patient Dob, String
job this.patientId = patientId; this.patientName patientName;
this.patientDob patientDob;=
this.patientEmail =patientEmail;}
public Long get patientId() {}
return patientId;
public void setpatientId (Long patientId) {
patientId patientId; = }
public String getpatientName() {
return patientName;}
public void setpatient Name (String patientName) {
patientName patientName;
public Integer getpatientAge() {
return Period. between (patientDob, LocalDate.now()).getYears(); }
public void patientAge (Integer patientAge) { patientAge patientAge; =}
public LocalDate getpatientDob() { return patientDob;}
public void setpatientDob (LocalDate patientDob) { patientDob patientDob; = }
public String patientEmail() {
return patientEmail;}
public void Hospitalmanagementsystem Email(String patient Email) { patientEmail patientEmail; = }
@Override
public String toString() {
return "Hospitalmanagement{" +
"patientId=" + patientId +
', patientName='" + patientname + '\'
patientAge=" + patientAge +
patientDob=" + patientDob +
", patientEmail='" + patientEmail + '\'' +
'}';}}
applications.properties
spring.datasource.url=jdbc: postgresql://localhost: 5432/hosman_db
spring.datasource.username=postgres
spring.datasource.password=saiabi@123
spring.jpa.hibernate.ddl-auto-create-drop
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
spring.jpa.properties.hibernate.format_sql=true;’
App.js
import React from "react"
import './App.css';
import { Browser Router as Router, Route, Routes, Link} from "react-router-dom";
import HospitalmanagementComponent from
'./components/HospitalmanagementComponent/hospitalmanagementComponent';
import HeaderComponent from
"./components/HeaderComponent/HeaderComponent";
import HospitalmanagementComponent from
"./components/HospitalmanagementComponent/hospitalmanagementComponent"; import
hospitalmanagementComponent from "
'./components/HospitalmanagementComponent/hospitalmanagementnComponent";
function App() {
return (<Router>
<div className="container"> <HeaderComponent/>
<nav className="nav-menu">
<Link to="/">Home</Link>
<Link to="/admin/add" >Add Member</Link>
<Link to="/admin/delete" >Delete Member</Link></nav>
<Routes>
<Route exact path='/' element={<HospitalmanagementComponent/>}></Route>
<Route path='/admin/add' element={<HospitalmanagementComponent/>}></Route> <Route
path='/admin/delete' element={<HospitalmanagementComponent/>}></Route>
</Routes>
</div>
</Router>);}
export default App;
```
## OUTPUT:
![Hospital_management_system_output](https://github.com/Akalyaalex/Hospital_management_syte/assets/114275126/7c0d73f7-255a-4282-b74a-6c1682fe399b)



