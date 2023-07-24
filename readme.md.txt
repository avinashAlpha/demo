package prog;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;


public class Facebook_login {
public static void main(String[] args) throws InterruptedException {
	System.setProperty("webdriver.chrome.driver", "C:\\Users\\dell\\Desktop\\Avinash\\Automation\\Basicsamme\\drivers\\chromedriver.exe");
	WebDriver driver = new ChromeDriver();
	driver.manage().window().maximize();
	driver.get("https://www.facebook.com/login/");
	Thread.sleep(2000);

	WebElement username = driver.findElement(By.id("email"));
	username.sendKeys("6204369100");

	WebElement password = driver.findElement(By.id("pass"));
	password.sendKeys("17101998avi");
	
	WebElement login=driver.findElement(By.xpath("//button['Log in']"));
	login.click();
}
avinash is name my