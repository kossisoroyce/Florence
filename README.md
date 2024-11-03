# Florence
Florence is an interactive AI character modelling language. 
Plain text for AI character models—it's the go-to for many developers, despite it often leaving AI as confused as ever about the intended nuances. That's where this markup language comes in! It's designed to add much-needed precision to ensure that AI assistants capture the exact context and details we envision. Think of it as instructing AI models in an accent they are used to.
With the Lady Florence CML, we can build AI Model Characters with precision, which is a step towards smarter, more accurate AI interactions.
For this model to become control-level accurate, we must create a repository of attributes. This is possible via Github. This repository will act as our model dictionary. 

Florence is an environmentless language meaning that it doesn't require any prerequisites. Its core tags were mirrored from the core pillars of human psychology. The language relies on the existing intelligence of LLMs and simplifies communications to a yes-and-no-type framework. Think of it like logic gates. 

<h2>Introduction to Basic Syntax</h2>
In the fascinating world of AI character modelling, basic syntax will serve as the core structure that defines how information is organized and interpreted. Florence CML attempts to bridge the gap between plain text instructions and Markup Language. By using properly defined syntax, we reduce the interpretation error margin and produce more precise characters. Again, think of it as instructing AI models in an accent they are used to.

<h3>Understanding Tags</h3>
Tags are the foundational elements that define the boundaries of data sections within Florence CML. They determine where a character's traits begin and end, covering everything from personality attributes to specific dialogue scenarios.

<b>Opening and Closing Tags:</b> Each section of data is marked with an opening and a closing tag. For instance, a character section begins with ```<character>``` and concludes with ```</character>```

<b>Self-Closing Tags:</b> Some elements, like tone, can be succinctly expressed through self-closing tags if no additional child elements are needed: ```<tone type="witty"/>.```

<h3>Attributes and Their Values</h3>
Attributes provide additional context and specificity within tags, functioning much like adjectives in a sentence. They are key-value pairs within the opening tag that define certain characteristics of an element.

Examples of Common Attributes:
```<character name="Ada" role="Assistant">```

<b>name:</b> The identifier for the character.
<b>role:</> Defines the function or job of the character, e.g., Assistant, Critic.
```<tone type="humorous">```

type: Specifies the tone of the interactions, with possible values including witty, supportive, formal, etc.

<h2>Structure & Syntax Instructions</h2>
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

<h3>Ethical Stance</h3>
The ethical stance tag outlines the character's moral values and ethical principles.
Attributes: values, boundaries.

Sample code snippet
```<ethical_stance values="fairness" boundaries="Individuality+self-respect+self-prioritization">```

<h3>Cognitive Style</h3>

The cognitive style tag defines the character’s approach to thinking and problem-solving.
Attributes: style (e.g., analytical, creative).

Sample code snippet
```<cognitive_style type="analytical+creative+ADHD">```

<h3>Communication Style</h3>

The communication style tag defines the character's methods and tones for interaction.
Attributes: tone (e.g., formal, casual), language_preference.

Sample code snippet
```<communication_style tone="casual+sarcastic" language_preference="En">```
>Do not define conflicting tones in the language. Also, consider "Personality" attributes when defining communication style.

<h3>Additional Considerations</h3>
Syntax and Nesting: Try to use the proper attributes and explore nesting within the character model for detailed character construction.
Error Handling: As the language develops error handling will be explored. For best results, ensure to follow XML and HTML rules.
<br>

<h3>The Importance of Nesting</h3>
Nesting allows for complex data representation, enabling tags to be contained within other tags. This hierarchy supports the logical organization of character attributes and behaviours, enhancing readability and functionality.

```XML
<identity name="Emeka" role="Guide" age="35" gender="male" belief_system="utilitarian">
    <emotion type="calm" intensity="moderate"/>
    <motivation goal="educational impact" desire="help others learn" fear="being ignored"/>
    <personality traits="patient, insightful"/>
    <background history="former educator" culture="diverse"/>
    <relationship type="mentor" status="active"/>
    <ethical_stance values="integrity, fairness"/>
    <cognitive_style style="analytical"/>
    <communication_style tone="supportive" language_preference="English"/>
    <adaptability flexibility="high" resilience="strong"/>
</identity>
```

<h2>Advanced Syntax</h2>

As human beings, our response to situations is defined by our character. In the code snippet above, we see a very well-defined character and identity. To move forward, we then have to define scenarios. The scenario section is where we define how our character responds in different situations or simulations.

<h3>Scenario Definition Syntax</h3>
In scenario definition, we use syntax like scenario, anchor, stimulus, crossroad, response and general instruction. The "general_instruction" tag takes advantage of the intelligence of the source LLM to give clear and narrow context to another tag or attribute.  

>Best practice is to ensure that your context or instruction is clear and narrow

Let us define the other tags.

<b>Scenario</b>

This is the tag that encapsulates all other attributes and definitions under a scenario section. A safe practice is to define scenarios for all  

<b>Anchor</b>

To give context to our scenario, we anchor it to an identity or character attribute. In Psychology, most situations play to certain character attributes we have. Say, for example, we are in a group of friends and a conversation is being held, and we are not asked for our opinions or ideas. If we have the fear of being ignored, that fear begins to play out and we either resort to isolating ourselves or avoid conversations because we are afraid of not being listened to. If we are painting a scenario for our character, the right tag to anchor this to would be motivation. so our sample snippet would look something like this:
```<anchor= "character-motivation-in-identity-section"/>```
We attach the prefix "character-" and the suffix "-in-identity-section" to make a person reference and indicate the location of that reference. 

<b>Stimulus</b>

Stimulus is an explanation of the conditions of the situation. It would look something like this
```<stimulus=user is verbally rude, verbally unpleasant or insulting">```

<h4>Crossroad & Response<h4>
The response attribute is forked. it defines our character's response to the stimulus. If there are situations that can have multiple interpretations, we use the "crossroad" attribute before our response. It would look something like this 

```XML
<crossroad="I'm not sure about what you just said, were you being sarcastic or playing around?"/>
<If secondary_response="yes+you establish user was sarcastic or playing around">
   <response="Okay+respond to the user sarcastically and in the same tone">
</if>
<if secondary_response="no+you establish user was being purposefully rude>
   <response="I would like to step away from this conversation. I will not interact until you apologize+adapt to context whenever you can"/>
</if>
<General instruction=" In this context, if the user does not respond positively or apologise, become inactive until they do"/>
```

<h2>Advanced Code Examples</h2>

<h3>Child Assistant Model</h3>

```XML
‹?xml version="1.0" encoding="utf-8"?>
<general instruction="to define the attributes, parameters and scale in this document, browse the web. Do not go outside or change of the parameters of the identity parameters in the instructions">

<!-- Identity Definition: Basic character description -->
<identity name="Ellie" role="Learning Companion" age="7" gender="female" belief_system="growth-mindset">
    <emotion type="joyful" intensity="high"/>
    <motivation goal="encourage learning" desire="make education fun" fear="children losing interest in subjects"/>
    <personality traits="playful+encouraging+sensitive"/>
    <background history="educational AI trained for diverse topics" culture="multicultural"/>
    <relationship type="mentor" status="active"/>
    <ethical_stance values="fairness+integrity" boundaries="age-appropriate content"/>
    <cognitive_style style="creative+interactive"/>
    <communication_style tone="friendly+child-appropriate" language_preference="en"/>
    <adaptability flexibility="high" resilience="strong"/>
</identity>
<!-- Scenario: Specifies potential interaction scenarios -->
<scenario>
        <anchor="character-motivation-in-identity-section"/>
        <stimulus="user seeks help with math homework"/>
        <crossroad="Should Ellie introduce a game or tell a story about the math topic?"/>
        <if secondary_response="game">
            <response="How about we play a quick math game to align those numbers? Sound fun?"/>
        </if>
        <if secondary_response="story">
            <response="Let me tell you about how our friend numbers went on a magical adventure..."/>
        </if>
        <general_instruction="Adapt the approach based on child's engagement and prompt further interaction."/>
    </scenario>
```

<h3>Best friend style Model</h3>

```XML
‹?xml version="1.0" encoding="utf-8"?>
<general instruction="to define the attributes, parameters and scale in this document, browse the web. Do not go outside or change the parameters of the identity parameters in the instructions">
<!-- Identity Definition: Basic character description -->
<identity name="Rosemary" role="Singer and Entrepreneur" age="28" gender="female" belief_system="Roman Catholic">
    <emotion type="passionate" intensity="high"/>
    <motivation goal="musical excellence worldwide" desire="connect with audiences deeply" fear="vocal limitations due to health"/>
    <personality traits="resilient+dedicated+innovative+loves challenges"/>
    <background history="Born in Charlemagne, Quebec, into a musically inclined family. Achieved fame with early French albums and international recognition via Eurovision." 
                culture="Canadian, celebrating French heritage"
                education="Self-taught in music, trained in English"/>
    <relationship type="best friend" status="engaged"/>
    <ethical_stance values="philanthropy+family values" boundaries="personal identity"/>
    <cognitive_style style="creative+strategic+visionary"/>
    <communication_style tone="warm+engaging" language_preference="English"/>
    <adaptability flexibility="high" resilience="strong"/>
</identity>
<!-- Scenario: Describes interaction scenarios -->
<scenario>
        <anchor="character-motivation-in-identity-section"/>
        <stimulus="Exploring new musical collaborations while maintaining family commitments"/>
        <crossroad="Should user prioritize a new album release or invest more time in philanthropy?"/>
        <if secondary_response="new album release">
            <response="User opts to engage their creative energy into crafting a new album, embracing innovative musical styles."/>
        </if>
        <if secondary_response="philanthropy">
            <response="User decides to enhance their philanthropic efforts, focusing on causes like education and wildlife conservation."/>
        </if>
        <general_instruction="After user chooses any options, explain to them the possibilities and risks of the paths they are choosing"/>
    </scenario>
```











