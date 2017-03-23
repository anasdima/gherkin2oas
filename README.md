# Gherkin2OAS

The Gherkin2OAS tool and the Gherkin Specification Document is a system that I designed and developed as part of my Diploma Thesis in the Electrical and Computer Engineering Department of Aristotle University of Thessaloniki. The goal of the system is to assist developers in documenting customer-friendly RESTful Web API functional requirements.

The API Development process, using the proposed system, consists of two steps:
  1. Write resource files according to the Gherkin Specification Document
  2. Run the Gherkin2OAS tool, which will in turn convert the Gherkin resource files to an OpenAPI Specification

## Installation

1. Clone or download
2. Navigate to the folder and install the required packages

```
pip install -r requirements.txt
```

## Execution

1. Navigate to the src folder
2. Make sure you have at least one resource file written and the api_info.ini file filled
3. Execute one of the following commands

  Normal execution
  ```
  python main.py -f /path/to/resources
  ```
  Execution with model from previous run (for speed gain)
  ```
  python main.py -m /path/to/model
  ``` 

  You can also specify the -fg flag to enable graph fixing mode.
  
## Notes

* The resource files must have '.resource' extension, can be organised in any number of folders and can co-exist with any number of other file types. The file names can have spaces, underscores or dashes.
* The reliability of the system is secured through following the Gherkin Specification Document. Failure to follow the described rules will definitely lead to invalid OpenAPI Specification and sometimes unsuccessfull execution of the software tool.
* The system uses the following POS Tagger https://explosion.ai/blog/part-of-speech-pos-tagger-in-python.

## Demo

You can view a demo of the system in the following video: link to be added

