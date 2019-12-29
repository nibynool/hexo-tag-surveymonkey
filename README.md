# Hexo Tag: Survey Monkey

## What is it?

A tag interpreter for [Hexo](https://hexo.io) static site generator to add a `{% surveymonkey %}` template tag to
embed [SurveyMonkey](https://www.surveymonkey.com/) surveys in a post.

## Why does it exist?

I created this custom tag as I wanted to display SurveyMonkey surveys as posts on my personal blog.  Although I could
use the raw HTML code provided by SurveyMonkey, I am running Markdown validation and have specified that HTML is not
permitted in Markdown files.  This plugin forces me to maintain consistent formatting throughout the blog. 

## Installation

1. Run `npm i @nibynool/hexo-tag-survey-monkey` in your root Hexo directory.

## Usage

1. Create a survey on SurveyMonkey (you will need a SurveyMonkey account for this)
2. Go to the `Collect Responses` page of your survey
3. Add a `Website collector` and set its type to `Embedded Survey`
4. Extract the survey identifier from the `Installation Code` that is provided by SurveyMonkey
5. Add the tag within your markdown, replacing the example code below with your code:
   ```markdown
   {% surveymonkey tRaiETqnLgj758hTBazgdwfsQcRBeORVDT3pHSkUpQ6gBUexut_2BQeJK6JAMlqYdS %}
   ```
