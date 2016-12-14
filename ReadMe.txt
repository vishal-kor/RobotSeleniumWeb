Project: CreateSurveys


Sub-Modules:    1) Create.robot
                2) Resources/PO/AddQues.robot
                3) Resources/PO/AddThePageTitle.robot
                4) Resources/PO/CreateSurveys1.robot
                5) Resources/PO/LandingPage.robot
                6) Resources/PO/SigninAction.robot
                7) Resources/Common.robot
                8) Resources/SM_Creation.robot


Library:    1) Selenium2Library


Description:    1) Selenium2Library:
                                    Selenium2Library is a web testing library for Robot Framework.
                                    Prior to running test cases using Selenium2Library, Selenium2Library must be imported into your Robot test suite,Open Browser keyword must be used to open a browser to the desired location.
                                    All keywords in Selenium2Library that need to find an element on the page take an argument, either a locator or now a webelement.

                2) AddQues.robot:
                                robot file for adding question to the survey

                3) AddThePageTitle.robot:
                                        robot file for adding page title to the survey

                4) CreateSurveys1.robot:
                                        robot file for creating the survey, adding name of the survey

                5) LandingPage.robot:
                                    robot file to navigate to surveymonkey website

                6) SigninAction.robot:
                                    robot file to do sign in action on the website

                7) Common.robot:
                                robot file for opening and closing browser

                8) SM_Creation.robot:
                                    robot file specifying the keyword file (user-defined)

Run Test Case:

            Command:robot -d Results Tests/Create.robot
Run Last Failed Test case:

            Command:robot --rerunfailed Results/output.xml -d Results Tests/Create.robot

Pre-Requisites:     1) Install pip  command:sudo apt-get pip.
                    2) Install robot framework  command:pip install robotframework-ride
                    3) Install Pycharm IDE

TOOLS:
1) Rebot: Creates exactly same log and report files for specific test case.
Command: rebot Results/output.xml
         rebot --include Smoke --name Smoke_test Results/output.xml (create log n report file only for particular subset of test case)