# Change Management – Request Process Tracking

## What is Change Management?

Change management is a structured process used to control modifications to a network or IT system.  
It ensures changes are planned, approved, documented, and tracked to reduce risk and prevent outages.

## Why Change Management Matters

Networks are interconnected systems. A small configuration change can cause major disruptions.

Change management helps to:

- Prevent unexpected downtime
- Reduce security risks
- Maintain compliance
- Improve accountability
- Enable rollback if something fails

---

## Request Process Tracking

Request process tracking ensures that every network change follows a formal workflow and is documented from start to finish.

### Typical Change Process

1. **Request Submission**
   - A change request is submitted (e.g., firewall rule update, switch configuration change).
   - Includes reason, scope, and expected impact.

2. **Review and Approval**
   - Technical team or change advisory board (CAB) reviews the request.
   - Risks and dependencies are evaluated.
   - Approval is granted before implementation.

3. **Planning**
   - Define implementation steps.
   - Schedule maintenance window if needed.
   - Create rollback plan in case of failure.

4. **Implementation**
   - Perform the change according to documented steps.
   - Monitor system behavior during execution.

5. **Validation**
   - Verify that the change works as expected.
   - Confirm no unintended side effects.

6. **Documentation and Closure**
   - Record results.
   - Update network diagrams and documentation.
   - Close the change request.

---

## Key Concepts

- Always document changes.
- Always test before full deployment.
- Always have a rollback plan.
- Emergency changes should still be documented after implementation.

---

## Example

Change: Open port 443 on firewall for a new web server.

Without change management:
- Port opened without documentation.
- Security team unaware.
- Future audit flags unknown open port.

With change management:
- Request submitted and approved.
- Security impact reviewed.
- Change implemented during maintenance window.
- Documentation updated.

---

Change management reduces risk and ensures stability in network environments.
