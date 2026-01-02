# Salesforce Speaker Session Assignment

## Overview
This project implements a Speaker and Session management system in Salesforce.

## Objects Used
- Speaker__c
- Session__c
- Speaker_Assignment__c

## Relationships
- Speaker Assignment → Speaker (Lookup)
- Speaker Assignment → Session (Master-Detail)

## Business Requirement (Task 1)
A speaker should not be assigned to two sessions that overlap in time on the same date.

## Implementation
- Apex Trigger runs before insert and before update
- Apex Handler checks existing speaker assignments
- If overlapping time is detected, record save is blocked with an error

## UI Configuration (Task 2)
- Speaker record page customized using Lightning App Builder
- Speaker Assignments displayed as a related list
- Page activated as Org Default

## Result
- Back-to-back sessions are allowed
- Overlapping sessions are blocked with an error message

## Technology Used
- Salesforce Apex
- Triggers and Handler pattern
- Lightning App Builder
