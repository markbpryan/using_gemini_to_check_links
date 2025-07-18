# Using Gemini to check links

Use a combination of Gemini and browser automation to navigate through the links in a set of topics to check whether the destination contains an error or a mismatch between the link text and prominent text at the destination. 

For more details, see the [related blog](https://medium.com/google-cloud/managing-links-with-gemini-validating-for-semantic-correctness-links-9b1a7e76299f).

The repo contains two implementations of the solution:
* [**WebDriver based**](https://github.com/markbpryan/using_gemini_to_check_links/blob/main/using_gemini_to_check_links.ipynb) uses [WebDriver](https://www.selenium.dev/documentation/webdriver/) for browser automation.
* [**Playwright based**](https://github.com/markbpryan/using_gemini_to_check_links/blob/main/using_gemini_to_check_links_pw.ipynb) uses [Playwright](https://playwright.dev/) for browser automation.

When you run either notebook, you'll be prompted for a Google AI Studio API key. You can get an API key for free at [aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey). 

The notebooks have been tested running in [Colab](https://colab.research.google.com).

The notebooks ingest a CSV file (by default [this example](https://github.com/markbpryan/using_gemini_to_check_links/blob/main/input_urls.csv)) with the URLs of the topics whose links will be checked. The `test_dataset_url` variable specifies the location of this CSV file.

The notebook generates an interactive report where you can see which links have errors or mismatches associated with them. The report has the following format:

![Report](https://raw.githubusercontent.com/markbpryan/using_gemini_to_check_links/refs/heads/main/output_report.png)


