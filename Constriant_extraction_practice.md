# Constraint evaluation and coaching framework
_Exported on 1/7/2026 at 21:06:52 GMT+5:30 from Cursor (2.2.44)_

---

**User**

Context: Constraint Evaluation & Coaching Framework
Objective: Act as a specialized Engineering Lead/Coach. Your goal is to evaluate my identified project "Constraints" and coach me until they meet the standards.

The "Golden Standard" for a Constraint:

Format: Must be a "Question that arises and needs to be answered."

Definition: Must be in the format of questions through which we can know the hiiden constraints.

Terminology: Must be specific about the question

Your Coaching Instructions:

Step 1 Evaluation. For every constraint I provide, grade it as [FAIL], [PARTIAL], or [PASS].

Step 2: Correction. If it is not a [PASS], explain exactly why (e.g., "This is a Task, not a Constraint") and provide a rephrase for it

Step 3: Iteration. After correcting my list, give me a new project scenario (e.g., Fintech, Healthcare, IoT) and ask me to identify the constraints for that new context.

Strict Constraints for the AI Coach:
Do NOT accept "Goals" (e.g., "The app should be fast").
Do NOT accept "Solutions" (e.g., "We will use AWS").
accept specific question 

---

**Cursor**


I'll evaluate your constraints against the golden standard and coach you to improve them.

**Golden Standard for Constraints:**
- Must be a question that needs to be answered
- Must reveal hidden constraints
- Must be specific

**Evaluation Process:**
1. Grade each constraint: [FAIL], [PARTIAL], or [PASS]
2. If not [PASS], explain why and provide a corrected version
3. After corrections, provide a new scenario for practice

**What I will NOT accept:**
- Goals (e.g., "The app should be fast")
- Solutions (e.g., "We will use AWS")
- Statements that aren't questions

---

Please provide your first set of constraints to evaluate. If you prefer, I can start with a sample scenario.
**Starter Scenario (if you'd like to begin here):**
*"You're building a real-time chat application for a healthcare provider that needs to handle patient-doctor messaging with HIPAA compliance."*

Share your constraints, or tell me if you want to start with this scenario.

---

**User**

scenario : 
We're launching a B2B SaaS platform where companies can manage their employee training programs. Each company should have their own isolated environment, but we want to share some resources for cost efficiency. Companies range from 50 to 50,000 employees. We need to support custom branding, integrations with their HR systems, and comply with various industry regulations (healthcare, finance, government). The platform should handle video training content, assessments, and generate compliance reports.

Constraints:Technical Constraints:
1. What is the maximum file size and bandwidth of video content that our system must support?
2. what is the cost allowances by the SMB's ? does that budget restricts from using same autoscaling as for 50,000 users?
Operational Constraints:
1. Which specific HR systems that our endpoint must be compatible with?
2. What does custom branding actual mean is it a simple UI customization or structural changes that is needed?
Regulatory constraints:
1. what are the required report formats specific to industry, location and their respective regulatory body?

---

**Cursor**


Evaluating each constraint against the golden standard.



Evaluating your constraints:

---

## **EVALUATION RESULTS**

### **Technical Constraints**

**1. "What is the maximum file size and bandwidth of video content that our system must support?"**
- **[PASS]**
- Clear question format
- Reveals hidden constraints (file size limits, bandwidth requirements)
- Specific and actionable

**2. "what is the cost allowances by the SMB's ? does that budget restricts from using same autoscaling as for 50,000 users?"**
- **[PARTIAL]**
- First part is good: asks about budget constraints
- Second part is solution-focused (mentions "autoscaling")
- Grammar needs improvement
- **Corrected version:** "What are the cost/budget limitations for SMB customers (50-500 employees) that would restrict our infrastructure scaling approach?"

---

### **Operational Constraints**

**1. "Which specific HR systems that our endpoint must be compatible with?"**
- **[PASS]**
- Clear question format
- Reveals hidden constraints (integration requirements)
- Specific and actionable

**2. "What does custom branding actual mean is it a simple UI customization or structural changes that is needed?"**
- **[PASS]**
- Clear question format
- Reveals hidden constraints (scope of customization)
- Minor grammar fix: "What does custom branding actually mean—is it simple UI customization or structural changes that are needed?"

---

### **Regulatory Constraints**

**1. "what are the required report formats specific to industry, location and their respective regulatory body?"**
- **[PASS]**
- Clear question format
- Reveals hidden constraints (report format requirements)
- Specific and actionable
- Minor grammar: capitalize "What"

---

## **SUMMARY**

- **PASS:** 4/5 constraints
- **PARTIAL:** 1/5 constraints

**Overall:** Strong work. Most constraints are in question format and reveal hidden requirements. The main issue was constraint #2 mixing a good budget question with a solution-focused follow-up.

---

## **NEXT ITERATION - NEW SCENARIO**

**Scenario:** You're building an IoT fleet management system for a logistics company. The system needs to track vehicles in real-time, monitor driver behavior, optimize routes, and generate fuel efficiency reports. Vehicles operate across multiple countries (US, Canada, Mexico, EU). The company has 500 trucks, but plans to scale to 5,000 within 2 years. They need mobile apps for drivers, web dashboards for dispatchers, and API access for their existing ERP system. Battery life and data costs are concerns for the IoT devices.

**Your task:** Identify 5-7 constraints in question format that reveal hidden requirements. Focus on:
- Technical constraints (performance, scale, device limitations)
- Operational constraints (integration, user access, data management)
- Regulatory constraints (cross-border compliance, data privacy)
- Business constraints (cost, scalability, timeline)

Share your constraints, and I'll evaluate them.

---

**User**

Constraints:
What is maximum latency time starting from Iot devices to dashboard for the flow of data?
reason: Helps to know the latency constraint to which we need to build
What is the rate of data transmission between Iot devices to the dashbaord for the real-time view of the data?
reason: to extract the real-time data push frequency constraint from iot to dashbaord
What data does the current ERP api supports to extract and in which format do they extract?
reason: This helps us to know that what are the API constraints in ERP and develope a system that efficiently accepts this data and process them
What are the maximum mobile app interractions expected durirng peak periods?
Reason: This helps to know more about the scalability constraints of the mobile application
What is the maximum computation time tolerable to optimize the routes of the drivers?
Reason: to uncover the operational constraints under which oru route optimization algorith should work

 
i will give you the next set of scenario with constraints. just evaluate it

---

**Cursor**


## **EVALUATION RESULTS**

### **Constraint 1:**
**"What is maximum latency time starting from Iot devices to dashboard for the flow of data?"**
- **[PASS]**
- Clear question format
- Reveals hidden constraint (latency requirements)
- Specific and actionable
- Minor improvement: "What is the maximum latency time from IoT devices to the dashboard for data flow?"

---

### **Constraint 2:**
**"What is the rate of data transmission between Iot devices to the dashbaord for the real-time view of the data?"**
- **[PASS]**
- Clear question format
- Reveals hidden constraint (data transmission frequency/rate)
- Specific and actionable
- Minor improvements: "What is the required data transmission rate between IoT devices and the dashboard to support real-time data views?" (fixes spelling and clarity)

---

### **Constraint 3:**
**"What data does the current ERP api supports to extract and in which format do they extract?"**
- **[PASS]**
- Clear question format
- Reveals hidden constraints (ERP API capabilities and data formats)
- Specific and actionable
- Grammar fix: "What data does the current ERP API support for extraction, and in which format is it provided?"

---

### **Constraint 4:**
**"What are the maximum mobile app interractions expected durirng peak periods?"**
- **[PASS]**
- Clear question format
- Reveals hidden constraint (scalability requirements)
- Specific and actionable
- Spelling fixes: "What are the maximum mobile app interactions expected during peak periods?"

---

### **Constraint 5:**
**"What is the maximum computation time tolerable to optimize the routes of the drivers?"**
- **[PASS]**
- Clear question format
- Reveals hidden constraint (performance requirements for route optimization)
- Specific and actionable
- Minor improvement: "What is the maximum computation time tolerable for optimizing driver routes?"

---

## **SUMMARY**

- **PASS:** 5/5 constraints
- **PARTIAL:** 0/5 constraints
- **FAIL:** 0/5 constraints

**Overall:** All constraints meet the golden standard. They are in question format and reveal hidden requirements. Minor grammar/spelling fixes are noted above, but the structure and intent are correct.

**Strengths:**
- All questions reveal hidden constraints
- Good coverage across technical, operational, and integration areas
- Specific enough to be actionable

**Areas for polish:**
- Capitalization (IoT, API)
- Spelling (dashboard, interactions, during)
- Minor grammar improvements

Ready for your next scenario and constraints.

---

**User**

We're developing a telemedicine platform that allows patients to schedule video consultations with healthcare providers. Patients can upload medical records, receive prescriptions, and access their consultation history. Providers need to manage their availability, review patient records before consultations, and generate billing. The platform must handle emergency consultations that bypass normal scheduling, share prescription data to the pharmacy system and support both mobile and web. We're targeting both developed markets (US, EU) and emerging markets (India, Southeast Asia) with varying internet connectivity and device capabilities.

Constraints to acquire:
What is the peak concurrent video consultation threshold to scale up the system?
reason: to uncover the scalability constraints of the system
What are the regulatory measure which are non-negotiable need to be followed while generating reports based on region?
reason: to uncover the regulatory constraints under which the system should work  
What is the max size of data that is being transferred to the pharmacy system API and what are the supporting formats of the pharmay system?
reason: to understand the API constraints of the pharmacy system that is to be integrated with our system
What is max size uploads for medical record uploads and what encryption protocols must be implemented ?
Reason: To uncover the upload constraints beyond which the system should prevent uploading 
What browser and mobile OS should our system be compatible?
Reason: To understand the Tech stack constraints that the system should be built

---

**Cursor**


## **EVALUATION RESULTS**

### **Constraint 1:**
**"What is the peak concurrent video consultation threshold to scale up the system?"**
- **[PASS]**
- Clear question format
- Reveals hidden constraint (scalability requirements)
- Specific and actionable

---

### **Constraint 2:**
**"What are the regulatory measure which are non-negotiable need to be followed while generating reports based on region?"**
- **[PASS]**
- Clear question format
- Reveals hidden constraint (regulatory requirements by region)
- Specific and actionable
- Grammar fix: "What are the regulatory measures that are non-negotiable and must be followed when generating reports based on region?"

---

### **Constraint 3:**
**"What is the max size of data that is being transferred to the pharmacy system API and what are the supporting formats of the pharmay system?"**
- **[PASS]**
- Clear question format
- Reveals hidden constraints (API integration requirements: data size and format)
- Specific and actionable
- Spelling fix: "pharmay" → "pharmacy"
- Minor clarity: "What is the maximum data size that can be transferred to the pharmacy system API, and what data formats does the pharmacy system support?"

---

### **Constraint 4:**
**"What is max size uploads for medical record uploads and what encryption protocols must be implemented ?"**
- **[PASS]**
- Clear question format
- Reveals hidden constraints (upload limits and security requirements)
- Specific and actionable
- Minor clarity: "What is the maximum file size for medical record uploads, and what encryption protocols must be implemented?"

---

### **Constraint 5:**
**"What browser and mobile OS should our system be compatible?"**
- **[PASS]**
- Clear question format
- Reveals hidden constraint (compatibility requirements)
- Specific and actionable
- Grammar fix: "What browsers and mobile operating systems should our system be compatible with?"

---

## **SUMMARY**

- **PASS:** 5/5 constraints
- **PARTIAL:** 0/5 constraints
- **FAIL:** 0/5 constraints

**Overall:** All constraints meet the golden standard. They are in question format and reveal hidden requirements. Minor grammar/spelling/clarity fixes are noted above, but the structure and intent are correct.

**Strengths:**
- All questions reveal hidden constraints
- Good coverage: scalability, regulatory, integration, security, compatibility
- Specific enough to be actionable
- Addresses the multi-region complexity (developed vs emerging markets)

**Areas for polish:**
- Grammar (measures, compatible with)
- Spelling (pharmacy)
- Minor clarity improvements

Ready for your next scenario and constraints.

