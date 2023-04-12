<h1 align="center"><img width="75" src="https://cdn-icons-png.flaticon.com/512/6967/6967331.png"> Taxi Service <img width="75" src="https://cdn-icons-png.flaticon.com/512/6967/6967331.png"></h1>
<h3><img width="25" src="https://cdn-icons-png.flaticon.com/512/391/391181.png"> About project </h3>
This web application is designed to imitation taxi service. The user can add vehicle manufacturers, add car models, add drivers, connect drivers and cars
<h3><img width="25" src="https://cdn-icons-png.flaticon.com/512/10180/10180990.png"> Project structure</h3>
<ul>
  <li>controller
    <ul>
        <li>IndexController (<code>/index</code>) - show all</li>
        <li>LoginController (<code>/login</code>) - login page</li>
        <li>LogoutController (<code>/logout</code>) - invalidate current session</li>
        <li>car
            <ul>
                <li>AddCarController (<code>/cars/add</code>) - add car to DB</li>
                <li>AddDriverToCarController (<code>/cars/drivers/add</code>) - add a driver to the car</li>
                <li>DeleteCarController (<code>/cars/delete</code>) - delete the car from DB</li>
                <li>GetAllCarsController (<code>/cars</code>) - show all cars</li>
                <li>GetAllMyCurrentCarsController (<code>/drivers/cars</code>) - show user cars</li>
            </ul>
        </li>
        <li>driver
            <ul>
                <li>AddDriverController (<code>/drivers/add</code>) - add a driver to DB</li>
                <li>DeleteDriverControllerr (<code>/drivers/delete</code>) - delete the driver from DB</li>
                <li>GetAllDriversController (<code>/drivers</code>) - show all drivers</li>
            </ul>
        </li>
        <li>manufacturer
            <ul>
                <li>AddManufacturerController (<code>/manufacturers/add</code>) - add a manufacturer to DB</li>
                <li>DeleteManufacturersController (<code>/manufacturers/delete</code>) - delete the manufacturer from DB</li>
                <li>GetAllManufacturersController (<code>/manufacturers</code>) - show all manufacturers</li>
            </ul>
        </li>
    </ul>
  </li>
  <li>dao
    <ul>       
      <li>CarDaoImpl - handler of Car model to DB</li>
      <li>DriverDaoImpl - handler of Driver model to DB</li>
      <li>ManufacturerDaoImpl - handler of Manufacturer model to DB</li>            
    </ul>
  </li>
  <li>model
    <ul>
        <li>Car</li>
        <li>Driver</li>
        <li>Manufacturer</li>
    </ul>
  </li>
  <li>service    
    <ul>
        <li>AuthenticationServiceImpl - a class for user authentication</li>
    </ul>       
  </li>
  <li>filter
    <ul>
        <li>AuthenticationFilter - user authentication check</li>       
    </ul>
  </li>
  <li>resources - This folder has one file (<code>init_db.sql</code>) for initial database initialization</li>
  <li>webapp - Folder with all JSP and CSS files</li>
</ul>
<h3><img width="25" src="https://cdn-icons-png.flaticon.com/512/993/993515.png"> Used technologies</h3>
<ul>
    <li>JDK 19.0.2</li>
    <li>Maven 3.8.7</li>
    <li>JDBC 4.2</li>
    <li>MySql 8.0.32</li>
    <li>Java Servlets 4.0.1</li>
    <li>Apache Tomcat 9.0.73</li>
</ul>
<h3><img width="25" src="https://cdn-icons-png.flaticon.com/512/5243/5243423.png"> Getting Started</h3>
<li>Clone the repository to your computer</li>
<li>Run the SQL script from <code>resources/init_db.sql</code></li>
<li>Replace the values of the <code>URL</code>, <code>USERNAME</code>, <code>PASSWORD</code> and <code>JDBC_DRIVER</code> in <code>util/ConnectionUtil.java</code> with your values</li>
<li>Build the project using Maven: <code>mvn clean install</code></li>
<li>Deploy the generated WAR file to servlet container such as Tomcat</li>

<h3><img width="25" src="https://cdn-icons-png.flaticon.com/512/1995/1995571.png"> Author</h3>
Zhuravlev Ivan
