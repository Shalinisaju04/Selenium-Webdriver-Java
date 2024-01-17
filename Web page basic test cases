package webpageTestingBasicsPackage;

import static org.testng.Assert.assertEquals;

import org.openqa.selenium.By;
import org.openqa.selenium.WebElement;
import org.testng.annotations.Test;

public class WebpageTestingBasicsTestCase extends AbstractWebDriverTest {
	@Test
  public void testTitle() {
		
		driver.get("https://www.saucedemo.com/");
		String title = driver.getTitle();// getting the title of the page
		assertEquals("Swag Labs", title);// Verifying the title of the webpage

  }

	@Test
	public void testInformationAboutPage() {

		// VERIFYING THE DETAILS OF USER NAME FEILD
		driver.get("https://www.saucedemo.com/");
		WebElement userName = driver.findElement(By.id("user-name"));
		String userNameValue = userName.getAttribute("value");
		assertEquals("", userNameValue);
		String tagName = userName.getTagName();
		assertEquals("input", tagName);

		// VERIFYING THE DETAILS OF PASSWORD FEILD
		WebElement password = driver.findElement(By.id("password"));
		String passwordValue = password.getAttribute("value");
		assertEquals("", passwordValue);
		String tagNameOfPassword = password.getTagName();
		assertEquals("input", tagNameOfPassword);

		// VERIFYING THE DETAILS OF LOGIN BUTTON
		WebElement login = driver.findElement(By.id("login-button"));
		String loginValue = login.getAttribute("value");
		assertEquals("Login", loginValue);
		String tagNameOfLogin = login.getTagName();
		assertEquals("input", tagNameOfLogin);
	}
}

