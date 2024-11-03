# Florence
Florence is an interactive AI character modelling language. 
Plain text for AI character models—it's the go-to for many developers, despite it often leaving AI as confused as ever about the intended nuances. That's where this markup language comes in! It's designed to add much-needed precision to ensure that AI assistants capture the exact context and details we envision.
With the Lady Florence CML, we can build AI Model Characters with precision, which is a step towards smarter, more accurate AI interactions.
For this model to become control-level accurate, we must create a repository of attributes. This is possible via Github. This repository will act as our model dictionary. 

Florence is an environmentless language meaning that it doesn't require any prerequisites. Its core tags were mirrored from the core pillars of human psychology. The language relies on the existing intelligence of LLMs and simplifies communications to a yes-and-no-type framework. Think of it like logic gates. 

<h2>Structure & Syntax</h2>
<b>Tags:</b> Similar to HTML, you can use opening and closing tags to define sections.

<b>Attributes:</b> Use attributes within tags to specify additional information, like ```<tone type="witty">``` to indicate tone.

<b>Nesting:</b> Allow tags to be nested for complex character definitions, ensuring logical grouping and hierarchy.

<h3>dictionary</h3>
A dictionary serves as a repository for the definitions of our attributes. For a broad stroke approach, we can set the model to browse the web and learn {this approach is not advised}.
Each character should have its dictionary. This is to modulate responses for extreme control levels.<b>[extreme control levels should be used for products serving children and young adults]</b>

<b>How to call the dictionary</b> 
To call the dictionary, you can use advanced functions like web_search="google.com" or call_home="URL to the dictionary on GitHub, or a web page" 

To define an attribute from a repository, attach "call_home" as a class. eg ```<relationship type="best-friend" Parameter_call_home="best-friend">```

<h3>Identity</h3>
The Identity tag Defines the core of the character, including basic identifiers and beliefs.
Attributes: name, role, age, gender, belief_system.

#sample code snippet
```<identity name="luna" role"house-keeper" age"25" gender="female" belief_system="Buddhist">```

<h3>Emotion</h3>
#<emotion>
The emotion tag conveys the character's emotional state or typical mood.
Attributes: type (e.g., joyful, anxious, calm), intensity.
*Use case: type="joyful"> can be used for products serving infants or young children*

Sample code snippet
```<emotion type="calm" intensity="stable">```

<h3>Motivation</h3>
The motivation tag highlights the driving forces behind a character's actions and decisions.
Attributes: goal, desire, fear.

Sample code snippet
```<motivation goal="Iron ore trading billionaire" desire="a quiet life" fear"mediocrity">```

<h3>Personality</h3>
The personality tag encapsulates the character's personality traits, influencing their behaviour and interactions.
Attributes: traits (e.g., introverted, optimistic).

Sample code snippet
```<personality traits="Extroverted+Optimistic+Kind+patient+">```
You can add more personality traits within the definition. make sure to use the + sign!


<h3>Background</h3>
The Background tag provides the context or backstory necessary to define the character's present state.
Attributes: history, education, culture.

Sample code snippet
```<background history="entry-level mining executive who grew up in wealth" culture="obnoxious" education="Havard MBA"/>```

<h3>Relationship</h3>
The relationship tag defines the nature of the character’s connections with its user.
Attributes: type (e.g., friend, mentor), status.

Sample code snippet
```<relationship type="friend" Parameter_call_home="friend">```



