{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "9e134966",
   "metadata": {},
   "source": [
    "# Project 1: SAT and ACT Test Analysis"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "9c7bec4f",
   "metadata": {},
   "source": [
    "## Problem Statement\n",
    "***\n",
    "\n",
    "In this project, I will be examining and exploring the trends in SAT and ACT participation rates and the aggregate scores in 2017, 2018 and 2019 after the change in SAT format in March 2016. As the participation rates vary greatly by states, the objective would be to identify trends and patterns to propose to College Board for the states to target to improve SAT participation rates. In addition, the SAT scores for the intended majors would be explored to idenfity if there are any trends for the scores in 2017, 2018 and 2019.\n",
    "\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "5e96835e",
   "metadata": {},
   "source": [
    "## Executive Summary and Recommendations\n",
    "***\n",
    "\n",
    "The trends analyzed from the data is that for a test with high participation rate for one test will usually mean a low participation rate for the other test. Hence, those states with mandatory ACT testing should not be targeted to improve SAT participation rates as the measures taken would likely not be effective. \n",
    "\n",
    "Test scores and participation rates of the tests stayed largely similar between the years of 2017 to 2019 where the states that score well will continue to score well in the following years. The test scores for a test are negatively correlated with the participation rates of the test.\n",
    "The SAT test scores for an intended major and number test takers stayed largely similar between the years of 2017 to 2019.  There is almost no correlation between the number of test takers and the SAT scores for an intended major in the same year.\n",
    "\n",
    "Based on the examined data, the recommendations would be to target California and Virginia for the states to improve SAT participation rates due to no mandatory testing policy, high population density and large population to increase the effectiveness and efficiency of the measures taken. Proposed measures that can be implemented include reducing the cost of SAT test and providing access to study and practice resources for potential students. "
   ]
  },
  {
   "cell_type": "markdown",
   "id": "79eb724c",
   "metadata": {},
   "source": [
    "## Data Dictionary\n",
    "***\n",
    "\n",
    "|Feature|Type|Dataset|Description|\n",
    "|---|---|---|---|\n",
    "|state|object|ACT scores/SAT scores|This value is the state in the United States of America.|\n",
    "|sat_participation_2017|float|SAT scores|This value refers to the participation rate of the SAT test in 2017.| \n",
    "|sat_participation_2018|float|SAT scores|This value refers to the participation rate of the SAT test in 2018.| \n",
    "|sat_participation_2019|float|SAT scores|This value refers to the participation rate of the SAT test in 2019.| \n",
    "|act_participation_2017|float|ACT scores|This value refers to the participation rate of the ACT test in 2017.| \n",
    "|act_participation_2018|float|ACT scores|This value refers to the participation rate of the ACT test in 2018.| \n",
    "|act_participation_2019|float|ACT scores|This value refers to the participation rate of the ACT test in 2019.| \n",
    "|total_score_2017|int|SAT scores|This value refers to the total score of the SAT test in 2017.| \n",
    "|total_score_2018|int|SAT scores|This value refers to the total score of the SAT test in 2018.| \n",
    "|total_score_2019|int|SAT scores|This value refers to the total score of the SAT test in 2019.| \n",
    "|composite_score_2017|float|ACT scores|This value refers to the total composite score of the ACT test in 2017.|\n",
    "|composite_score_2018|float|ACT scores|This value refers to the total composite score of the ACT test in 2018.|\n",
    "|composite_score_2019|float|ACT scores|This value refers to the total composite score of the ACT test in 2019.|\n",
    "|intended_college_major|object|SAT Majors Scores|This value is the college major that the students intend to enter when taking the SAT test.| \n",
    "|test_takers_ 2017|int|SAT Majors Scores|This value shows the number of students taking the SAT test in 2017.| \n",
    "|test_takers_ 2018|int|SAT Majors Scores|This value shows the number of students taking the SAT test in 2018.|\n",
    "|test_takers_ 2019|int|SAT Majors Scores|This value shows the number of students taking the SAT test in 2019.|\n",
    "|percent_2017|float|SAT Majors Scores|This value is the percent of the students choosing that particular intendedmajor over the total student population in 2017.| \n",
    "|percent_2018|float|SAT Majors Scores|This value is the percent of the students choosing that particular intendedmajor over the total student population in 2018.| \n",
    "|percent_2019|float|SAT Majors Scores|This value is the percent of the students choosing that particular intendedmajor over the total student population in 2019.| \n",
    "|total_2017|int|SAT Majors Scores|This value is the total score of the SAT for that particular major in 2017.| \n",
    "|total_2018|int|SAT Majors Scores|This value is the total score of the SAT for that particular major in 2018.| \n",
    "|total_2019|int|SAT Majors Scores|This value is the total score of the SAT for that particular major in 2019.| \n"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.8.8"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
