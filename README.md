# sel
from selenium import webdriver
from selenium.webdriver.common.by import By
import time

driver=webdriver.Chrome()
driver.get("http://localhost/login.do")
driver.find_element(By.CSS_SELECTOR,"[type='checkbox']").click()
time.sleep(5)
driver
.find_element(By.CSS_SELECTOR,"[type='checkbox']").click()
driver.maximize_window()
time.sleep(5)
driver.minimize_window()
time.sleep(5)
driver.close()
driver.quit()
