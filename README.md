# AUTOSAR Debugging Automation

An AI-assisted debugging workflow for AUTOSAR customer error logs.  
The system ingests incoming failure artifacts, compares scenario paths against a known baseline, identifies the first deviation and last meaningful reached state, generates structured root-cause hypotheses with next-check recommendations, and produces dashboard-backed RCA summaries with human-in-the-loop review.

## What it does
- Parses customer error scenarios and baseline paths
- Detects path deviations and ErrorHandler transitions
- Extracts structured debugging signals such as first deviation, missing baseline states, and failure region
- Uses an AI agent to generate likely causes, observations, and recommended next checks
- Produces readable RCA summaries and dashboard links for developer review
- Supports human approval before sending/debug handoff

## Current scope
This version focuses on first-pass RCA automation for AUTOSAR state-path debugging.  
A planned next enhancement is historical case retrieval (RAG) to compare new failures against similar previously analyzed incidents.
