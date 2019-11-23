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
### Test Case 2: 
```
```

### Test Case 3: 
```
```

### Test Case 4: 
```
```

### Test Case 5: 
```
```

### Test Case 6:
```
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
