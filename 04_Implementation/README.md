# Implementation

## Project Title
Implement Client Script & UI Policy (Incident)

## Implementation Details

The project is implemented in ServiceNow using Client Script and UI Policy on the Incident table.

## Client Script Implementation

A Client Script named "Prevent state change via list edit" is implemented on the Incident table.

### Configuration
- Table: Incident
- Type: onCellEdit
- Field: State
- Active: Yes

### Function
The Client Script prevents users from changing the Incident State through list editing and displays an alert message.

## UI Policy Implementation

A UI Policy named "High Impact Control" is implemented on the Incident table.

### Condition
- Impact is 1 - High

### UI Policy Actions
- Urgency
- Assignment Group

The UI Policy controls the Incident form fields when the Impact is set to High.

## Result

The Client Script and UI Policy work successfully on the Incident form and apply the configured rules based on the user's actions.
