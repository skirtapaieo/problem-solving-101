# problem-solving-101

In many situations, starting from interviews, onboarding, working in groups, and individually, with larger team constellations and so on it is very important to have a clear and understandable problem solving process, that is being followed consistently, and when side-steps are done they are done in an aware manner. 

In all the other repositories, we are trying to have a proper problem solving approach, documented in the README.MD for each repository. We are not very good at documenting side-steps from it and sometimes time does not allow for it at all. 

This expanded problem-solving process provides a more comprehensive view, starting from why the problem is worth solving, through how to solve it, and finally, how to validate the solution.

Lets have the tournament winner problem as an example. 

## Step 1 - Need identification (Why) 

This is the stage where you identify the need for solving a problem. You consider the impact of the problem, who it affects, and why it's worth solving. 
For instance, in the tournament problem, the need could be "There is a requirement for a fair and efficient system to determine the winner in a series of games or competitions."

> **Team note:** At this stage, gather requirements from stakeholders. These could be product managers, customers, business analysts, or other relevant parties. Understand why the problem is important to them, what their needs are, and how solving the problem would add value. This stage may involve meetings, surveys, or user research to better understand the needs and constraints.

## Step 2 - Problem Definition (What)

Here, you would articulate the specific problem you're trying to solve based on the identified need. In the tournament problem, this step would involve stating that you need to find the team with the most points, with each win granting three points.

> **Team note:** Based on the needs and requirements gathered, define the problem. Make sure the problem statement aligns with the stakeholders' understanding. 

## Step 3 - Conceptual Understanding (When)

It's important to understand the specific circumstances or context in which the problem exists. This could include understanding when the problem occurs, under what conditions, and any constraints that exist. In the tournament problem, the context could be "The solution should work for any number of teams and games, and should handle ties appropriately."

> **Team note:** Understand the context in which the problem exists. This could involve understanding the user journey, existing system architecture, business rules, and regulations, etc. Also, consider the design or user interface (UI) elements that might affect the solution. 

## Step 4 - Conceptual Solution (How)

This is where you devise a conceptual or theoretical solution to the problem. It might not be the final solution, but it forms a basis to start the actual problem-solving process. Here a simple example of pseudocode could help to make things clearer earlier. 

```pseudocode
1. Initialize an empty dictionary to keep track of the points of each team.
2. For each competition in the competitions list:
     1. Determine the winner of the competition (home team if result is 1, away team if result is 0).
     2. If the winner is not in the points dictionary, add them with a score of 0.
     3. Add 3 points to the winner's score in the points dictionary.
3. Find the team with the maximum points in the points dictionary.
4. Return the team with the maximum points as the tournament winner.
```

> **Team note:** Come up with a high-level solution. This can involve brainstorming sessions with different teams, including design and product teams. Sketch out rough UI designs or system diagrams if necessary.

## Step 5 - Discuss Solution Alternatives (Hows) 

Discuss and evaluate potential alternative solutions to the problem.

> **Team note:** Evaluate different solution paths. Consider technical feasibility, design aesthetics, user experience, cost, time, and other factors. This stage may involve getting feedback from different stakeholders. 

## Step 6 - Initial Approach/Drafting

Once a solution is chosen, a prototype or draft solution is created.

> **Team note:**  Start drafting the solution. For software problems, this would involve writing pseudocode or actual code. For design problems, this could involve creating wireframes or design mockups.

## Step 7 - Optimization/Finalization

After testing and refining the initial draft, the solution is optimized and finalized.

> **Team note:** Refine and optimize your solution. For a design problem, this might mean making the design more intuitive and aesthetically pleasing. For a coding problem, this might involve optimizing your code for efficiency.

## Step 8 - Validation

Finally, the solution is tested with various test cases to ensure its correctness and efficiency.

In the case of testing it is very good to have clear names on testing scenario for everyone to understand the intentions. 

```python 
# Test Case 1: Basic Input ...
competitions = [["A", "B"], ["B", "C"], ["C", "A"]]
results = [1, 1, 1]
assert tournamentWinner(competitions, results) == "B"

# Test Case 2: One Team wins all matches ... 
competitions = [["A", "B"], ["A", "C"], ["A", "D"]]
results = [1, 1, 1]
assert tournamentWinner(competitions, results) == "A"

```

> **Team note:** Test your solution to ensure it meets all requirements and performs as expected. This could involve unit testing for code, usability testing for designs, and getting final approval from stakeholders.

## Step 9 - Implementation and Review 

> **Team note:** Implement the solution and gather feedback. This could involve deploying the code, launching a new feature, or rolling out a new design. After implementation, review the solution with stakeholders to ensure it meets their needs and expectations. 
> 
> By involving stakeholders at each step and considering design and product aspects, you ensure the solution you develop meets the needs of the end users and aligns with the goals of your organization.

## Step 10 - It is a marathon not a sprint 

### Psychological safety 

Psychological safety is a crucial aspect in any collaborative environment, especially in diverse teams working on complex problems. It's the shared belief that a team is safe for interpersonal risk-taking, meaning members feel comfortable expressing their thoughts, ideas, and concerns without fear of negative consequences.

In the context of a multi-team environment, promoting psychological safety can have several benefits:

- Fosters Open Communication: When team members feel psychologically safe, they are more likely to share their thoughts, ask questions, seek help, and discuss problems openly. This can lead to better problem-solving and decision-making.

- Encourages Innovation: A psychologically safe environment encourages people to take risks and come up with innovative solutions. It allows for trial and error without fear of punishment, which can drive creativity and innovation.

- Improves Learning and Growth: Psychological safety allows team members to admit mistakes and learn from them, leading to personal growth and overall team improvement.

E nhances Team Collaboration: When team members feel safe and respected, they are more likely to collaborate effectively, trust each other, and work towards shared goals.

To promote psychological safety in a multi-team environment, you can consider the following strategies:

- Promote Respect and Fairness: Encourage team members to treat each other with respect and fairness. This includes listening attentively to others' ideas, avoiding harsh criticism, and promoting equality.

- Encourage Open Communication: Create an environment where team members feel free to express their thoughts, ask questions, and share their ideas.

- Normalize Mistakes: Frame mistakes as opportunities for learning, not as failures. This can encourage team members to take risks and innovate without fear of retribution.

- Show Empathy and Understanding: Be understanding and empathetic to team members' challenges. Recognize that everyone can have off days and that personal circumstances can affect work performance.

- Lead by Example: Leaders should model the behavior they want to see in their team. If leaders show vulnerability, admit their own mistakes, and encourage open communication, team members are more likely to do the same.

Implementing these strategies can help create a psychologically safe environment where all team members feel comfortable contributing to their full potential.





