# Automation-project2023
Selenium Automation-project2023 
from selenium import webdriver 

from selenium.webdriver.common.keys import Keys 

driver = webdriver.Chrome("C:\chromedriver_win32\chromedriver.exe")

driver.get("https://www.testbirds.de")
    
newelement=driver.find_element_by_css_selector('a[href$="/home/tester"]')

newelement.click()

list_of_forms = driver.find_elements_by_css_selector('form')
second_form = list_of_forms[1] 

new_element=second_form.find_element_by_css_selector('input[name="firstname"]')
new_element.click()
new_element.send_keys("Mirela")

new_element=second_form.find_element_by_css_selector('input[name="lastname"]')
new_element.click()
new_element.send_keys("Blaschke")


new_name=second_form.find_element_by_name('username')
new_name.click()
new_name.send_keys("MirelaB")

list_of_countries=second_form.find_element_by_css_selector('div[class="Select-placeholder"]')
list_of_countries.click()

sleep
new_name=second_form.find_elements_by_css_selector('div.Select_menu_outer>*')
print(new_name)

