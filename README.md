# 2019-ITCS473-Shabu
## Selenium Web Driver project
### Testing Techniques
* Selenium
* Python

Tested website : https://smartedu.mahidol.ac.th/Authen/login.aspx

### Test Case 1: Username and Password are Correct (Valid Input)
```
def TestCase1(driver):
    driver.set_page_load_timeout(10)
    driver.get("https://smartedu.mahidol.ac.th/Authen/login.aspx")
    driver.find_element_by_name("txtStudentcode").send_keys("u5988036")
    driver.find_element_by_name("txtPassword").send_keys("Bomb5988036")
    driver.find_element_by_class_name("btnStdLogin").send_keys(Keys.ENTER)
    time.sleep(5)
    driver.quit()
    print 'TestCase1 Completed'
    return;
```
### Test Case 2: Username and Password are Incorrect (Valid Input)
```
def TestCase2(driver):
    driver.set_page_load_timeout(10)
    driver.get("https://smartedu.mahidol.ac.th/Authen/login.aspx")
    driver.find_element_by_name("txtStudentcode").send_keys("u6388036")
    driver.find_element_by_name("txtPassword").send_keys("Bomb12345")
    driver.find_element_by_class_name("btnStdLogin").send_keys(Keys.ENTER)
    time.sleep(5)
    driver.quit()
    print 'TestCase2 Completed'
    return;
```

### Test Case 3: For the student who did not have Student ID
```
def TestCase3(driver):
    driver.set_page_load_timeout(10)
    driver.get("https://smartedu.mahidol.ac.th/Authen/login.aspx")
    driver.find_element_by_class_name("btnNewStudent").send_keys(Keys.ENTER)
    driver.find_element_by_name("txtNewStudentcode").send_keys("u6388036")
    driver.find_element_by_name("txtIdNumber").send_keys("1101476354882")
    driver.find_element_by_class_name("btnNewStdLogin").send_keys(Keys.ENTER)
    time.sleep(10)
    driver.quit()
    print 'TestCase3 Completed'
    return;
```

### Test Case 4: Identify StudentID for Students who are freshmen or newcoming
```
def TestCase4(driver):
    driver.set_page_load_timeout(10)
    driver.get("https://smartedu.mahidol.ac.th/Authen/login.aspx")
    driver.find_element_by_class_name("btnMenuCheckStudentId").send_keys(Keys.ENTER)
    driver.find_element_by_name("txtIdCard").send_keys("1101476354883")
    driver.find_element_by_class_name("btnSearchStudentId").send_keys(Keys.ENTER)
    time.sleep(10)
    driver.quit()
    print 'TestCase4 Completed'
    return;
```

### Test Case 5: Swap Website Language from "Thai to English" and "English to Thai"
```
def TestCase5(driver):
    driver.set_page_load_timeout(10)
    driver.get("https://smartedu.mahidol.ac.th/Authen/login.aspx")
    driver.find_element_by_class_name("btnEn").send_keys(Keys.ENTER)
    driver.find_element_by_class_name("btnTh").send_keys(Keys.ENTER)
    time.sleep(10)
    driver.quit()
    print 'TestCase5 Completed'
    return;
```

### Test Case 6: Click on an image hyperlink
```
def TestCase6(driver):
    driver.set_page_load_timeout(10)
    driver.get("https://smartedu.mahidol.ac.th/Authen/login.aspx")
    driver.find_element_by_xpath("//img[@src='images/BANNER_MUGE_TH.png']/parent::a").send_keys(Keys.ENTER)
    time.sleep(10)
    driver.quit()
    print 'TestCase6 Completed'
    return;
```

### Test Case 7:
```
```

### Test Case 8:
```
```

### Test Case 9:
```
```

### Test Case 10:
```
```
