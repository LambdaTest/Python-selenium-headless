# How to set browser specific options in Python-selenium on [LambdaTest](https://www.lambdatest.com/?utm_source=github&utm_medium=repo&utm_campaign=Python-selenium-headless)

If you want to set browser specific options for an automation test in Python-selenium on Lambdatest, you can use the following steps. You can refer to sample test repo [here](https://github.com/LambdaTest/python-selenium-sample).

# Steps:

You can specify the various browser specific options in the test file capabilities section. The following is an example on how to set Chrome specific options using chromeOptions in capabilties:


```python
desired_caps = {
            'LT:Options': {
                "build": "Python Demo",  # Change your build name here
                "name": "Python Demo Test",  # Change your test name here
                "platformName": "Windows 11",
                "selenium_version": "4.0.0",
                "chromeOptions" : {
                "args" : ["incognito"]  # ChromeOption to start chrome in incognito mode
                
            },
            "browserName": "Chrome",
            "browserVersion": "98.0",
        }

```

## Step 4: Run your test

```bash
python lambdatest.py
```

# Links:

[LambdaTest Community](http://community.lambdatest.com/)

