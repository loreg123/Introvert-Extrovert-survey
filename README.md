# Introvert-Extrovert-survey


1. Do you feel energized when you are around a lot of people?

    <input type="radio" id="yes1" 
name="question1" value="yes">
    <label for="yes1">Yes</label><br>
    <input type="radio" id="no1" name="question1" value="no">
    <label for="no1">No</label><br>
    

2. Do you often find yourself lost in your thoughts?

    <input type="radio" id="yes2" 
name="question2" value="yes">
    <label for="yes2">Yes</label><br>
    <input type="radio" id="no1" name="question2" value="no">
    <label for="no2">No</label><br>

3. Do you prefer working in a team or alone?

    <input type="radio" id="yes3" 
name="question3" value="yes">
    <label for="yes3">Yes</label><br>
    <input type="radio" id="no3" name="question3" value="no">
    <label for="no3">No</label><br>

4. After attending a social event, do you feel the need to spend time alone to recharge?

 <input type="radio" id="yes4" 
name="question4" value="yes">
    <label for="yes4">Yes</label><br>
    <input type="radio" id="no4" name="question4" value="no">
    <label for="no4">No</label><br>
    
5. Are you comfortable being the center of attention?

    <input type="radio" id="yes5" 
name="question5" value="yes">
    <label for="yes5">Yes</label><br>
    <input type="radio" id="no5" name="question5" value="no">
    <label for="no5">No</label><br>

6. Do you often reflect on your feelings and thoughts?

    <input type="radio" id="yes6" 
name="question6" value="yes">
    <label for="yes6">Yes</label><br>
    <input type="radio" id="no6" name="question6" value="no">
    <label for="no6">No</label><br>

7. Do you prefer having a wide circle of friends or a few close ones?

   <input type="radio" id="yes7" 
name="question7" value="yes">
    <label for="yes7">Yes</label><br>
    <input type="radio" id="no7" name="question7" value="no">
    <label for="no7">No</label><br>

8. Do you feel drained after social interactions, even if you enjoyed them?

    <input type="radio" id="yes8" 
name="question8" value="yes">
    <label for="yes8">Yes</label><br>
    <input type="radio" id="no8" name="question8" value="no">
    <label for="no8">No</label><br>

9. Do you enjoy engaging in small talk with strangers?

<input type="radio" id="yes9" 
name="question9" value="yes">
    <label for="yes9">Yes</label><br>
    <input type="radio" id="no9" name="question9" value="no">
    <label for="no9">No</label><br>
    
10. Do you often engage in self-reflection or daydreaming? 

    <input type="radio" id="yes10" 
name="question10" value="yes">
    <label for="yes10">Yes</label><br>
    <input type="radio" id="no10" name="question10" value="no">
    <label for="no10">No</label><br>

11. Do you feel more fulfilled after spending time with others or by yourself?

<input type="radio" id="yes11" 
name="question11" value="yes">
    <label for="yes11">Yes</label><br>
    <input type="radio" id="no11" name="question11" value="no">
    <label for="no11">No</label><br>
  
12. You more likely to express your opinions in a group setting or keep them to yourself?

 <input type="radio" id="yes12" 
name="question12" value="yes">
    <label for="yes12">Yes</label><br>
    <input type="radio" id="no12" name="question12" value="no">
    <label for="no12">No</label><br>
    
13. Do you prefer attending large parties or small gatherings?

    <input type="radio" id="yes13" 
name="question13" value="yes">
    <label for="yes13">Yes</label><br>
    <input type="radio" id="no13" name="question13" value="no">
    <label for="no13">No</label><br>

14. Does spending an entire day alone sound enjoyable or boring to you?

<input type="radio" id="yes14" 
name="question14" value="yes">
    <label for="yes14">Yes</label><br>
    <input type="radio" id="no14" name="question14" value="no">
    <label for="no14">No</label><br>
    
15. Do you often initiate conversations in social settings?

    <input type="radio" id="yes15" 
name="question15" value="yes">
    <label for="yes15">Yes</label><br>
    <input type="radio" id="no15" name="question15" value="no">
    <label for="no15">No</label><br>

16. Are you more focused on your inner world or the world around you? 

   <input type="radio" id="yes16" 
name="question16" value="yes">
    <label for="yes16">Yes</label><br>
    <input type="radio" id="no16" name="question16" value="no">
    <label for="no16">No</label><br>

17. Do you prefer deep conversations with a few people over casual chats with many? 

<input type="radio" id="yes17" 
name="question17" value="yes">
    <label for="yes17">Yes</label><br>
    <input type="radio" id="no17" name="question17" value="no">
    <label for="no17">No</label><br>
    
18. Do you often feel the need to take breaks from social interaction?

    <input type="radio" id="yes18" 
name="question18" value="yes">
    <label for="yes18">Yes</label><br>
    <input type="radio" id="no18" name="question1" value="no">
    <label for="no18">No</label><br>

19. Are you quick to adapt to social situations?
 
<input type="radio" id="yes19" 
name="question19" value="yes">
    <label for="yes19">Yes</label><br>
    <input type="radio" id="no19" name="question19" value="no">
    <label for="no19">No</label><br>
    
20. Do you often spend time exploring your thoughts and feelings through writing, art, or other solitary activities?
 
    <input type="radio" id="yes20" 
name="question20" value="yes">
    <label for="yes20">Yes</label><br>
    <input type="radio" id="no20" name="question20" value="no">
    <label for="no20">No</label><br>

# HTML template
html_template = f"""
<!DOCTYPE html>
<html>
<head>
<title>Introvert or Extrovert Survey</title>
</head>
<body>
<h2>Introvert or Extrovert Survey</h2>
<form action="SUBMIT_LINK" method="post">
"""

# Adding questions and options to the HTML template
for i, question in enumerate(survey_questions, 1):
    html_template += f"""
    <p>{i}. {question}</p>
    <input type="radio" id="yes{i}" name="question{i}" value="yes">
    <label for="yes{i}">Yes</label><br>
    <input type="radio" id="no{i}" name="question{i}" value="no">
    <label for="no{i}">No</label><br>
    """

# Closing the HTML form
html_template += """
<input type="submit" value="Submit">
</form>
</body>
</html>
"""

html_template.strip()  # Removing leading/trailing whitespaces

# Save this HTML content to a file
html_file_path = "/mnt/data/introvert_extrovert_survey.html"
with open(html_file_path, "w") as file:
    file.write(html_template)

html_file_path
