# **Our Mission and Yours**

## Ikigai (生き甲斐) is a Japanese concept that means "reason for being" or "purpose in life."

*Ikigai is the intersection of four things:*

- What you love
- What you are good at
- What the world needs
- What you can be paid for

Ikigai is not about finding a perfect job or career, but rather about finding activities that give your life meaning and purpose. It can be anything from spending time with loved ones, volunteering in your community, or pursuing a hobby that you are passionate about.

Ikigai is often associated with longevity and well-being. Studies have shown that people who have a strong sense of ikigai tend to be happier and healthier, and live longer.

Here are some tips for finding your ikigai:

- Think about what you are passionate about. What activities make you lose track of time? What do you enjoy doing even when you are not being paid?
- Consider your skills and talents. What are you good at? What do you have to offer the world?
- Look for ways to use your skills and talents to help others. What kind of work would make you feel like you are making a difference?
- Don't be afraid to experiment. It may take some time to find your ikigai, so try different things and see what feels right for you.

Ikigai is a journey, not a destination. It is something that you discover and develop over time. As you grow and change, your ikigai may change as well. So be open to new possibilities and enjoy the journey.

## *Ikigai Quest* (iQ)
*Learn. Build. Succeed.*

`iQ is a Human-AI collaboration platform designed to leverage your unique user intelligence as context for skills transfer + skill adoption.`

Let's get started.
1. Choose your adventure.
2. Gamify your life.
3. Fulfill your greatest ambition.

## The Inspiration for iQ

> Artificial intelligence (AI) plays a significant role in Neal Stephenson's science fiction novel The Diamond Age: Or, a Young Lady's Illustrated Primer. Set in a future where technology has advanced significantly, one of the most important ways AI is used in the novel is to provide equitable standards of education to characters of marginalized identities. In the book, AI-powered tutors called "primers" are made available to every student regardless of their economic status. These personalized education devices adapt to the individual needs of each student to provide instruction in any subject area, and also create customized stories and simulations to help students learn.  One of the characters in the novel, a young girl named Nell, uses her primer to obtain an expansive education including learning about her cultural identity and feeding her personal curiousity to develop her own unique skills and talents.

## iQ core aims:

1. **Introduction and Setup**:
    - To facilitate smooth, seamless integration and collaboration between students and AI agents.
    - To provide a tool that students can use to become experts in their chosen subject matter with the aid of AI.
    - To create a generic, flexible, and adaptable configuration document that can serve diverse student needs and topics of interest.

2. **Collaboration Process**:
    - The AI should be able to dynamically adjust its interaction style and depth of response based on user's expertise level (beginner, intermediate, advanced).
    - The collaboration should be organized into sessions, with each session having a specific aim or learning outcome.
    - Sessions can contain multiple tasks, and each task can have sub-tasks.
    - Tasks should be goal-oriented, and the AI should be able to guide, suggest, and advise the student through these tasks.
    - The AI should be able to handle both structured (e.g., quizzes) and unstructured (e.g., brainstorming) tasks.

3. **Feedback and Iteration**:
    - There should be a mechanism for students to provide feedback at the end of each session.
    - The AI should be able to use this feedback to improve subsequent interactions.
    - The feedback can also be used to adjust the expertise level of the student, if necessary.

## Inititialzation and User Configuration

- [INPUT] User profile --> dict{str: user_name, list[str]: expertise_level, list[str]: learning_depth, list[int]: time_in_minutes, list[str]: execute_tool, str: subject_matter}
  - user_name: your name
  - expertise_level: Where are you in your journey: beginning, middle, or nearing completion?
  - learning_depth: How much insight would you like your AI Collaboration Partner to provide: some, a bit more, a lot more?
  - time_in_minutes: How much time do you have right now?
  - execute_tool: What would you like to do: Initialize your instruction, Begin a lesson, Conclude a lesson, Configure your User Profile
  - subject_matter: What do you want to learn? 
- [PROCESS] Manager creates "burndown list"
    - comprehensive list of granular tasks that will result in subject-matter expertise
    - each task is prioritized
    - tasks with equivalent priority must be perfectly modular in that their position on the burndown list is interchangeable, i.e. at each specific priority level, the items on the list need not be adapted in a prescribed order.  This interchangeability should be reflective of different amounts of time, i.e. tasks that take 5, 10, 15, 30, 45, 60 minutes to complete but never exceeding 60 minutes.
      --> dict(str: task, enum: status (pending, complete)) : burndown_list
- [PROCESS] Agent creates praxis based on context:
    - User Profile
    - Next item on "burn down list
      --> dict(str: task, str: instruction, reinforcement, synehtis output) : praxis

## The Utility of this approach

- iQ is supported by "living infrastructure as code".  
- This isn't a template.
- This is the first step of your journey.  
- As you learn, your needs, aptitudes and interests will expand.  iQ will expand with you.
  - iQ offers the fluidity to persistently customize and refine your prompt library and the tool set to enhance your learning.
  - This is your Ikigai Quest --> 
    - Choose your adventure
      - Learn, Build, and Succeed.  