# Using Gemini to check links

Use a combination of Gemini, browser automation and glue code to navigate through all the links in a set of topics to check whether the destination contains an error or a mismatch between the link text and prominent text at the destination. 

The repo contains two implementations of the solution:
* [**WebDriver based**](https://github.com/markbpryan/using_gemini_to_check_links/blob/main/using_gemini_to_check_links.ipynb) uses [WebDriver](https://www.selenium.dev/documentation/webdriver/) for browser automation.
* [**Playwright based**](https://github.com/markbpryan/using_gemini_to_check_links/blob/main/using_gemini_to_check_links_pw.ipynb) uses [Playwright](https://playwright.dev/) for browser automation.

The notebook ingests a CSV file (by default [this example](https://github.com/markbpryan/using_gemini_to_check_links/blob/main/input_urls.csv)) with the URLs of the topics whose links will be checked. The `test_dataset_url` variable specifies the location of this CSV file.

The notebook generates an interactive report where you can see which links have errors or mismatches associated with them. The report has the following format:

![Report](https://raw.githubusercontent.com/markbpryan/using_gemini_to_check_links/refs/heads/main/output_report.png)


