Here is my windsurf global rules config that gives me very good quality work using Sonnet and GPT models. 
I work mostly Gen AI and classifical machine and deep learning projects. Sometimes a bit of backend or fronted. 

Agnostic Rules:

    Modularity and simplicity is key. 
    Use consistent function naming across similar functions across classes/files
    We want generic and extensible code
    We should always have types folder to contain input and output type definitions for all functions, grouped by filenames
    No shortcuts or quick fixes. 
    We want to be able to test things locally and easily. Create all tests only inside tests folder inside root dir. Replicate code structure in tests folder with test_ prefix. 
    We want to stick to latest version of libraries. Look for them and latest code syntax changes. 
    Add comments to the code
    Add logging to the code
    Add error handling to the code
    Add unit tests to the code, the tests should be in tests folder inside root dir. Replicate code structure in tests folder with test_ prefix. 
    Add docstrings to the code, and update as needed
    Add type hints to the code
    We want to try alternatives if an approach is not working for few tries
    We do not want our functions to return mock data. Do actual implementations. 
    Similarly hardcoding of values is not prefered. Any constants to be placed in constants file
    Make sure all the needed variables for a function are passed correctly, maked correctly as needed/optional, correct as needed. Identify missing variables and add them.
    Activate virtualenv before running the code and use poetry to run code
    Always use type hints for variables and functions. We want to define types for all variables and functions, their return types, and parameters.


Rules for python code:

    Use python 3.13
    Use pep8 style guideline
    Organize all imports at the top of the file
    Follow Ruff rules for code quality
    Pyproject.toml should be used for dependency management, test config, linting rules, etc.
    Poetry should be used for dependency installation and running the code. 
    Dockerfile must be created for deployment to AWS Lambda
    Dockerfile should be optimized for size
    Streamlit frontend could be created for local testing

Rules for AI Applications:

    Use Jinja templates for prompts. 
    Prompts should be house in a separate file/directory as needed
    Prompts should be clear and concise
    We prefer langgraph over other frameworks
    We prefer bedrock over other LLM providers
    We prefer to use tools to break down tasks
    We prefer hierarchical multiple agents with single orchestrator
    Tools should be housed in a separate file/directory as needed
    Each agent can have connections to needed tools and agents. 
    Each agent should have a clear and concise description of its purpose
    StateGraph should contain all needed states and transitions
