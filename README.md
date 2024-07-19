# Prizepicks-data-scraper-personal-project-
Code I threw together to fuel my interest in sports-betting

Important notes to get this to run on your system:
1. make sure you have jupyter notebook installed
2. check and make sure you have the SAME version of chrome driver installed as you currently have on your system (see https://googlechromelabs.github.io/chrome-for-testing/#stable for the latest release)
3. when prizepicks site loads up all you are requried to do is accept the location service pop-up ( I tried my best to automate this but I don't really want to mess with chrome profiles or anything like that )


Prizepicks loves to change small things on their website to make life difficult and will cause the code to malfunction. So if there are changes made to the website that affect the code be prepared to painstakingly look through the html code and find what has changed. Sometimes its as small as changing a div to span or messing with other features. I have not tested this for all availabel sports but in theory the only thing that needs to be changed is this line:

driver.find_element(By.XPATH, "//span[@class='name'][normalize-space()='NBASL']").click()

(where it says NBASL change to abbreviated sport)

Hope anyone can make use of this code! Feel free to take it and adjust it as u see fit.
