# DemoOne
@BeforeClass,@ AfterClass
package testing;

import org.testng.annotations.AfterClass;
import org.testng.annotations.AfterMethod;
import org.testng.annotations.BeforeClass;
import org.testng.annotations.BeforeMethod;
import org.testng.annotations.Test;

public class ClassOne {
	
	@BeforeClass
	public void CreateDatabaseConnection() {
		System.out.println("Creating Database connection with Preprod.");
	}
	
	@AfterClass
	public void CloseDatabaseConnection() {
		System.out.println("Closing the Database Connection.");
	}
	
	@BeforeMethod
	public void Login() {
		System.out.println("Login to the application.");
	}
		
	@AfterMethod
	public void Logout() {
		System.out.println("Logout of the application.");
	}
	
	@Test
	public void CreateNewModuleRequest() {
		System.out.println("Create New Module Request.");
	}
	
	@Test
	public void ApproveModuleRequest() {
		System.out.println("Approve Module Request.");
	}
	
	

}
