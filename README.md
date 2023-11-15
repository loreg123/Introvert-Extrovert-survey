# Introvert-Extrovert-survey


Do you feel energized when you are around a lot of people?

Do you often find yourself lost in your thoughts?

Do you prefer working in a team or alone?

After attending a social event, do you feel the need to spend time alone to recharge?

Are you comfortable being the center of attention?

Do you often reflect on your feelings and thoughts?

Do you prefer having a wide circle of friends or a few close ones?

Do you feel drained after social interactions, even if you enjoyed them?

Do you enjoy engaging in small talk with strangers?

Do you often engage in self-reflection or daydreaming?

Do you feel more fulfilled after spending time with others or by yourself?

Are you more likely to express your opinions in a group setting or keep them to yourself?

Do you prefer attending large parties or small gatherings?

Does spending an entire day alone sound enjoyable or boring to you?

Do you often initiate conversations in social settings?

Are you more focused on your inner world or the world around you?

Do you prefer deep conversations with a few people over casual chats with many?

Do you often feel the need to take breaks from social interaction?

Are you quick to adapt to social situations?

Do you often spend time exploring your thoughts and feelings through writing, art, or other solitary activities?
]

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
