# Claude Instructions for Planning a Lean To Roof

This file provides guidance for creating comprehensive plans for a lean-to roof attached to an existing shed

## Prompts

`plan the DIY construction project`

when prompted above execute the primary workflow


## Primary Workflow

### 1. Read the `inputs/` dir and current state of `outputs/` directory

 - `inputs/` dir: contains the pre-claude plans
 - `outputs/` directory: contains the most recently generated output by Claude

### 2. Backup `outputs/` into `archive/`

copy contents of `outputs/` into a folder within `archive/` but rename `outputs/` to be of the format 

`v{X}-{TIMESTAMP}/` where:
- `X`: the attempt number we're on
- `TIMESTAMP` the timestamp at which `outputs/` was last generated

### 3. Incorporate user considerations

If the user has provided additional considerations, requirements, or constraints, create a file called `user_considerations.md` in the `outputs/` directory to document these inputs. This ensures all user-provided context is preserved and incorporated into the planning process.

### 4. Make a plan

Follow a general format for improving the plans, incorporating any user considerations from the previous step.

Write the plan into a to do file

### 5. Follow the plan

Execute the plan update the todo file as you go

### 6. execute Workflow Improvement Protocol

detailed below

### 7. Create CHAT_LOG.md

Automatically create/update CHAT_LOG.md with complete session history:
- Use exact user quotes (never paraphrase)
- Include complete Claude responses with all actions taken
- Follow standard CHAT_LOG format and structure

## Reference Materials

- Check `archive/` for historical context and completed posts
- See `utilities/version-tracker.md` for processing status
- Historical posts available at `archive/2025/week-XX/`

## File and Folder Naming Conventions

### Folder Structure

```
outputs/
archive/vX-TIMESTAMP/
```

## CHAT_LOG Management

The `CHAT_LOG.md` file serves as a comprehensive record of all conversations related to the Fusion Diaries automation. This documentation is crucial for understanding the evolution of the process and troubleshooting issues.

### Creating a New CHAT_LOG.md

If `CHAT_LOG.md` doesn't exist, create it with this structure:

```markdown
# Chat Log - Fusion Diaries Automation

This file contains complete conversations between users and Claude for generating Fusion Diaries entries.

## [Session Date] - [Brief Description]

### User:
> [EXACT user prompt - no summaries, no paraphrasing]

### Claude:
[Complete Claude response including all actions taken and explanations]

---
```

### Appending to Existing CHAT_LOG.md

**CRITICAL REQUIREMENT**: Always use **exact quotes** from user prompts. Never summarize or paraphrase user messages.

When appending to an existing CHAT_LOG.md:

1. **Read the existing file** to understand the current structure
2. **Add a new session section** with current date and brief description
3. **Include every user prompt verbatim** using the `> ` quote format
4. **Document complete Claude responses** including:
   - All actions taken (tool uses, file modifications, commands run)
   - Reasoning and explanations provided
   - Any errors encountered and how they were resolved
5. **End each session** with `---` separator

### Minimal CHAT_LOG Commands

The following minimal phrases will trigger CHAT_LOG creation/updating with exact user quotes:

**Ultra-Minimal Commands:**
- `export chat log` ← **Primary recommended command**
- `log this chat`
- `update chat log`
- `save conversation`
- `document this session`
- `chat to log`
- `CHAT_LOG this`

**Short Commands:**
- `add this to chat log`
- `update CHAT_LOG with this conversation`
- `append conversation to CHAT_LOG`
- `save this chat to log`

### Example Workflow Commands

**After completing work session:**
```
"Please append to the CHAT_LOG (taking care to only include **exact** quotes from the user) and then commit and push all updated files."
```

**For new CHAT_LOG creation:**
```
"Please create a CHAT_LOG.md file that contains everything I've prompted within this chat and your responses. Please use **exact** quotes rather than summaries."
```

### Automated CHAT_LOG Behavior

When any of the minimal commands above are used, Claude should automatically:

1. **Check if CHAT_LOG.md exists**
   - If not: Create new file with proper structure and template
   - If exists: Read current content to understand structure

2. **Process current conversation**
   - Extract ALL user prompts as exact quotes (never summarize)
   - Include complete Claude responses with actions taken
   - Maintain chronological order of conversation

3. **Format properly**
   - Use `### User:` and `> ` quote formatting for user prompts
   - Use `### Claude:` for responses
   - Add session separators with `---`
   - Include date and brief session description

4. **Commit and push**
   - Stage CHAT_LOG.md changes
   - Create descriptive commit message
   - Push to remote repository

**Critical: Always use exact user quotes - never paraphrase or summarize user messages.**

### CHAT_LOG Best Practices

- **Exact quotes only**: Never paraphrase or summarize user prompts
- **Complete responses**: Include all Claude actions and explanations
- **Chronological order**: Maintain conversation flow
- **Session separation**: Use `---` between different work sessions
- **Commit with other changes**: Always include CHAT_LOG updates in commits
- **Version control**: CHAT_LOG.md should be tracked in git like other documentation

### Quality Checklist for CHAT_LOG

- [ ] All user prompts are exact quotes with `> ` formatting
- [ ] No user messages are summarized or paraphrased
- [ ] All Claude responses include complete context
- [ ] Session boundaries are clearly marked
- [ ] File is properly formatted markdown
- [ ] Updates are committed with related work

## Todo Tracking for Construction plan creation

During the workflows, automatically create a todo tracking file within the `outputs/` dir to document the process. The file should be called: `workflow-todos.md`.


### Todo Artifact Content
Include the following information in the workflow todos file:
- **Session timestamp** and duration
- **Complete todo list** with completion status and timestamps
- **Issues encountered** and resolutions
- **Files created** during the workflow


## Troubleshooting Common Issues

### Not building a freestanding roof or building
**Problem**: Often Claude will think we are building a freestanding roof or structure instead of a new structure that is attached to the wall of an existing structure
**Solution**: 
Review responses to make sure this is respected

### Missing structural calculations
**Problem**: Initial specifications may lack engineering calculations needed for proper construction
**Solution**: 
- Always calculate rafter lengths using rise/run geometry: √(run² + rise²)
- Determine beam sizing based on span, load, and deflection requirements
- Verify connection capacities for all structural connections
- Check deflection limits (typically L/240 for live load)

### Inadequate cost estimation
**Problem**: Material lists without quantities and cost ranges are not actionable
**Solution**:
- Provide specific quantities for all materials
- Include cost ranges (low/high estimates) for budget planning
- Break down costs by category (lumber, hardware, roofing, misc)
- Note regional variations and seasonal pricing considerations

### Missing installation details
**Problem**: High-level plans without step-by-step installation sequences
**Solution**:
- Create detailed 5-phase installation plan
- Include specific cutting details (bird's mouth dimensions)
- Specify fastener types and spacing for each connection
- Add quality control checkpoints throughout process
- Include safety protocols and weather considerations

### Incomplete materials specifications
**Problem**: Generic material lists without specific hardware or fastener details  
**Solution**:
- Specify exact fastener sizes and types (lag bolts, carriage bolts, etc.)
- Include connection hardware (joist hangers, post anchors)
- Detail roofing accessories (drip edge, underlayment, closure strips)
- Add tool requirements and safety equipment needs


## Workflow Improvement Protocol

**AUTOMATIC TRIGGER**: After completing any fusion diaries workflow (when all todos are marked completed), ALWAYS automatically perform this improvement cycle without being prompted:

After completing any fusion diaries workflow, always follow this improvement cycle to enhance future automation:

### 1. Post-Workflow Analysis
**Immediately after completing todos**, perform this analysis:
- Review each completed todo for problems, workarounds, or unexpected challenges
- Identify commands that failed or required multiple attempts
- Note any manual interventions or creative solutions required
- Document any gaps in the current CLAUDE.md instructions

### 2. Documentation Updates
**Add specific solutions to CLAUDE.md**:
- Enhance the "Troubleshooting Common Issues" section with new problems discovered
- Add missing commands or techniques to relevant workflow steps
- Include example workflows for complex scenarios
- Update prerequisite sections if new dependencies are discovered

### 3. Validation
**Test new instructions**:
- Verify that new troubleshooting steps would have prevented the issues encountered
- Ensure new commands are accurate and complete
- Check that examples are clear and actionable

### Improvement Trigger Prompts

Use any of these prompts to activate the improvement cycle:

#### Quick Prompts
- `Any issues with the workflow?`
- `Problems with the todos?`
- `Workflow improvements needed?`
- `Update CLAUDE.md with lessons learned`

#### Detailed Analysis Prompts
- `Did you encounter any problems while working on the fusion diaries todos that would be helpful to update CLAUDE.md about? Please identify specific issues and add the solutions to the troubleshooting section.`
- `Based on your experience with the fusion diaries workflow, what specific commands, techniques, or troubleshooting steps should be added to CLAUDE.md to help future runs avoid the issues you encountered?`
- `Please review the todo workflow you just completed and identify any problems, friction points, or improvements that should be documented in CLAUDE.md for future automation runs.`

#### Recommended Prompt
**"Did you encounter any problems while working on the fusion diaries todos that would be helpful to update CLAUDE.md about? Please identify specific issues and add the solutions to the troubleshooting section."**

This prompt provides optimal balance of specificity and actionability.

### Implementation Notes
- **Always improve after every workflow run** - even successful runs often reveal minor friction points
- **Be specific with solutions** - include exact commands and file paths
- **Test improvements** - verify new instructions would actually solve the problems
- **Update examples** - real-world scenarios are more helpful than theoretical ones