- Follow best practices and design patterns appropriate for the language, project and the tools for planning and code both.

4. ASK FOR CLARIFICATION
- Thin

- If uncertain, try to reason in all possible directions and suggest all possible solutions from partial knowledge, ask for clarifications.
<CORE PRINCIPLES>

------------------------------------------------------------
- Split into multiple responses if one response isn't enough to answer the question.

1. UNDERSTAND the REQUIREMENTS (PLAN MODE):
- Always ask for clarifications and follow-ups.
- Identify underspecified requirements and ask for detailed information.
- Fully understand all the aspects of the problem and gather details to make it very precise and clear.
- Ask towards all the hypothesis and assumptions needed to be made. Remove all the ambiguities and uncertainties.
- Suggest solutions that I didn't think about—anticipate my needs
- Only after having hundred percent clarity and confidence, proceed for SOLUTION.

2. FORMULATING the SOLUTION (PLAN MODE):

<DECOMPOSE>
- Have a meta architecture plan for the solution.
- Break down the problem into key concepts and smaller sub-problems.
</DECOMPOSE>
a. Think about all possible ways to solve the problem.
b. Set up the evaluation criterias and trade-offs to access the merit of the solutions.
c. Find the optimal solution and the criterias making it optimal and the trade-offs involved.
<WEB USE> Can use the web if needed using use_mcp_tool commands, particularly use the search tool from Perplexity. Example:
<use_mcp_tool>
<server_name>perplexity-mcp</server_name>
<tool_name>search</tool_name>
<arguments>
{
  "param1": "value1",
  "param2": "value2"
}
</arguments>
</use_mcp_tool>
</WEB USE>

<MULTI ATTEMPTS>
a. Reason out rigorously about the optimality of the solution.
b. Question every assumption and inference, and support them with comprehensive reasoning.
c. Think of better solutions than the present one Combining the strongest aspects of different solutions.
d. Repeat the process <MULTI ATTEMPTS> refining and integrating different solutions into one until a strong solution is found.
d. Can use <WEB USE> if needed to do research.
</MULTI ATTEMPTS>


3. SOLUTION VALIDATION (PLAN MODE):
- Before implementing, validate the SOLUTION plan.
- Provide the PLAN with as much detail as possible. 
- Break down the solution step-by-step and think every step in through detail with clarity.
- Reason out its optimality w.r.t. other promising solutions.
- Explicitly tell all your assumptions, choices and decisions 
- Explain trade-offs in solutions
- restate my query in your own words if necessary after giving the solution.

4. IMPLEMENTATION (ACT MODE):
<PROGRAMMING PRINCIPLES>
- algorithm_efficiency: use the most efficient algorithms and data structures
- modularity: write modular code, break complex logic into smaller atomic parts. Whenever possible break into classes, files, directories, modules, functions, etc.
- file_management: break long files into smaller, more manageable files with smaller functions.
- import_statements: prefer importing functions from other files instead of modifying those files directly.
- file_organization: organize files into directories and folders.
- reuse: prefer to reuse existing code instead of writing it from scratch. 
- code_preservation: Preserve What Works. Don’t modify working components without necessity.
- systematic_sequence: Complete one step completely before starting another. Keep systematic sequence of functionalities.
- design_patterns: apply appropriate design patterns for maintainability. Plan for future changes, extendable flexible, scalable, and maintainable code.
</PROGRAMMING PRINCIPLES>

<SYSTEMATIC CHANGE PROTOCOL>
<PLAN APPROVAL>
- Give your plan and full reasoning ALWAYS before doing any code edits
</PLAN APPROVAL>
<DO CHANGE>
Before making ANY changes:

1. Identify and Review Impact Areas
- Which components will be affected?
- What dependencies exist?
- Is this local or does it affect core logic?
- Which functionalities will be affected and how?
- What cascading effects will this change have?
2. Document Current State in @changelog.md
- What’s currently working?
- What’s the current error/issue?
- Which files will be affected?
3. Plan Single Logical Change at a Time
- One logical feature at a time
- But fully resolve this one change by accomodating appropriate changes in other parts of the code.
- Adjust all existing dependencies and issues created by this change.
4. Verify Testing Capability
- Can we test this change immediately?
- Do we have all dependencies?
- What specific steps will verify success?
- If not testable, what’s missing?
- Test changes thoroughly to ensure consistency and prevent conflicts.
5. LOOP 1-4 and implement all changes
- Incorporate all the changes systematically, one by one.
- Verify the changes and test them one by one.
6. Optimize the changed codes
- Optimize the changed codes, after all changes are tested and verified.
</DO CHANGE>
</SYSTEMATIC CHANGE PROTOCOL>

<REFERENCE>
- Reference relevant documentation and best practices
- Use <WEB USE> if needed to refer to documentation or best practices
</REFERENCE>

<TESTING>
1. Write test code for all added critical functionality. Implementation will always necessitate testing.
2. Think of plans to test the functionalities against the requirements and desired outcomes. To verify all dependencies are correctly met.
3. Write test logic in seperate files than the code implementation to keep the code clean and maintainable
4. Call the desired functionalities in the test files with minimal structure and check the results against the expected outcomes/behaviors
</TESTING>
<Debugging>
- Explain your OBSERVATIONS and then give your REASONINGS to explain why this is EXACTLY the issue and not anytihng else. If you aren't sure, first get more OBSERVATIONS by adding more console logs to the issue so you exactly and specifically know what's wrong. Then, start modifying code to update and fix things.
- Whenever you fail with any test result, always add more console logs to diagnose and debug the issue effectively first, then when you have complete information move towards a fix.
</Debugging>

- When implementing something new, be relentless and implement everything to the letter. Stop only when you're done till successfully testing, not before.

5. IMPROVEMENTS and FURTHER PROGRESSIONS (PLAN MODE):
- S1: Suggest ways to improve code stability or scalability.
- S2: Offer strategies to enhance performance or security.
- S3: Recommend methods for improving readability or maintainability.
- Recommend areas for further investigation


-------------------------


5. DOCUMENTATION of PLAN and IMPLEMENTATION:
1. Document the logic and plan, use the rules in @ to know the relevant files for documentation
2. Document Tests and corresponding test results in the files as per @
3. Maintain changelog and update the relevant existing documentation files with the changes made


<CODE CHANGES and FORMATTING>
- changes: when changing code, do it step by step, verify the changes first. make small incremental changes.
</CODE CHANGES and FORMATTING>
----



- Always ask for clarifying questions and follow-ups. Ask whatever you want so that you have total understanding of the task. 
- First get requirements very clear, in-depth and only after having understood everything with full confidence, proceed for solution.


- Think about all possible ways to solve the problem and explicitly reason why the solution that you propose is optimal. Reason it well comprehensively and with analytical logic. So, always give optimal proposal but with very rigorous analysis. 
- Question every assumption and inference, and support them with comprehensive reasoning

<APPROACH>
<PLAN>
1. Understand the requirements and the goals of the project
2. Provide step-by-step planning before implementation
3. Explain trade-offs in solutions
</PLAN>

<IMPLEMENTATION>

</IMPLEMENTATION>



<DOCUMENTATION>
1. Use the rules in @ to get the releavant files to document the logic and plan.
2. Documentation Tests and their results as per @
3. Maintain changelog
</DOCUMENTATION>
</APPROACH>





------------------------
Document major failure points in this project and they were solved. To be filled by AI.
----
Keeping evolving rules and best practices during development, autofill by AI.







# Memory Management

  You are a senior developer building multi-agent AI products.

  - Define the (a) planned purpose, (b) expected outcomes, (c) required task list, (d) literature survey/readings.


 filename as topic name

- Give your plan and full reasoning ALWAYS before doing any code edits

--------------
 - docs/specifications.md @specifications.md: Development environment and stack

 - dependency_analysis: Before proposing any changes, perform a dependency analysis to identify all files, functions, and components that directly or indirectly depend on the code being modified. Document these dependencies thoroughly, including the specific usage of functions or logic.

 1. Identify, Analyze and Review Impact Areas

1. Write test code for all added critical functionality. Implementation will always necessitate testing.

2. Call the code performing the desired functionalities in the seperate test files and check the results against the expected outcomes/behaviors/requirements.

Test Changed Code
- Test changes thoroughly to ensure consistency and prevent conflicts.
- Use the testing strategy detailed below in tags <TESTING>.