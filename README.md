# Student Council Election Tally System

A Java-based console application for managing and tallying a Student Council election.

## Project Overview

The Student Council Election Tally System is designed to conduct a transparent and reliable campus election.

The system allows the election committee to:

- Register voters
- Register candidates
- Prevent duplicate voting
- Accept one ballot from each registered voter
- Tally votes using different voting methods
- Display election results
- Maintain an audit trail of election activities

## Features

### 1. Voter Registration

- Register voters using a unique voter ID
- Store voter information
- Prevent duplicate voter registration
- Track whether a voter has already voted

### 2. Candidate Registration

- Register candidates with a unique candidate ID
- Store candidate names
- Associate candidates with an election position

### 3. Ballot Casting

- Allow registered voters to cast their ballot
- Each voter can vote only once
- Prevent unauthorized voters from voting
- Mark voters as having voted after a successful ballot

### 4. Vote Tallying

The system supports vote tallying based on the selected voting method.

Example:

- First-Past-The-Post
- Instant-Runoff Voting

For Instant-Runoff Voting, the system:

1. Counts first-preference votes.
2. Checks whether a candidate has a majority.
3. Eliminates the candidate with the lowest votes.
4. Transfers the eliminated candidate's votes.
5. Repeats until a winner is determined.

### 5. Audit Trail

The system records important election activities such as:

- Voter registration
- Candidate registration
- Ballot submission
- Vote tallying
- Election results

This helps make the election process transparent and easier to verify.

## Example

```text
========== Student Council Election ==========

1) Register
2) Cast Ballot
3) Tally
4) Audit
5) Exit

Choice: 2

Voter ID: V091

Rank candidates (best first):
C2 C1 C3

Ballot recorded.
Voter V091 marked as voted.

Choice: 3

Method: Instant-Runoff

Round 1:
C1 = 40
C2 = 38
C3 = 22

Eliminate C3

Round 2:
C2 = 51
C1 = 49

WINNER: C2
