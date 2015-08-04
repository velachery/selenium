# selenium
//  SIR DIZ Z SHANAZ ,CODING BY XPATH AS U SAID..........
package shanazpack;

import org.apache.bcel.generic.Select;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.firefox.FirefoxDriver;

public class Shanazclass {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
WebDriver driver=new FirefoxDriver();
driver.manage().window().maximize();
driver.get("https://book.spicejet.com/register.aspx");
WebElement DAY=driver.findElement(By.xpath("//select@id='CONTROLGROUPREGISTERVIEW_PersonInputRegisterView_DropDownListDOBDay'"));
WebElement MONTH=driver.findElement(By.xpath("//select@id='CONTROLGROUPREGISTERVIEW_PersonInputRegisterView_DropDownListDOBMonth'"));
WebElement YEAR=driver.findElement(By.xpath("//select@id='CONTROLGROUPREGISTERVIEW_PersonInputRegisterView_DropDownListDOBYear'"));
driver.findElement(By.xpath("//input@id='CONTROLGROUPREGISTERVIEW_MemberInputRegisterView_TextBoxAgentUserName'")).sendKeys("SHANAZ");
driver.findElement(By.xpath("//input@id='CONTROLGROUPREGISTERVIEW_MemberInputRegisterView_PasswordFieldAgentPassword'")).sendKeys("ddd");
driver.findElement(By.xpath("//input@id='CONTROLGROUPREGISTERVIEW_MemberInputRegisterView_PasswordFieldPasswordConfirm'")).sendKeys("ddd");
WebElement title=driver.findElement(By.xpath("//select@id='CONTROLGROUPREGISTERVIEW_PersonInputRegisterView_DropDownListTitle'"));
driver.findElement(By.xpath("//input@id='CONTROLGROUPREGISTERVIEW_PersonInputRegisterView_TextBoxFirstName'")).sendKeys("shanaz");
driver.findElement(By.xpath("//<input@id='CONTROLGROUPREGISTERVIEW_PersonInputRegisterView_TextBoxLastName'")).sendKeys("fathima");
WebElement Nationality=driver.findElement(By.xpath("//select@id='CONTROLGROUPREGISTERVIEW_PersonInputRegisterView_DropDownListNationality'"));
Select obj1=new Select(DAY);
obj1.SelectByValue("5");
Select obj2=new Select(MONTH);
obj2.SelectByvisibleText("july");
Select obj3=new Select(YEAR);
obj3.SelectByIndex("23");
Select obj4=new Select(title);
obj4.SelectByvisibleText("online booking");
Select obj5=new Select(Nationality);
obj5.SelectByvisibleText("INDIA");




							


	}

}
