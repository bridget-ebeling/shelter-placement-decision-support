# Shelter Placement Decision-Support System

Locally run, privacy-focused decision-support tool for matching shelter animals to rescues. Built with AI assistance.

## Overview

This tool helps a county shelter find rescue placements for its animals. It combines intake criteria from multiple no-kill rescues into one searchable interface, so staff don't have to cross-check separate spreadsheets by hand. It also makes it easier to find rescues that can take medically or behaviorally complex animals.

**Deployed:** Dec 4, 2025

## The Problem

The shelter kept each rescue partner's intake criteria in separate spreadsheets, covering dogs, cats, horses and other species. To find a placement, staff had to compare an animal against every list by hand, checking:

- Species / breed
- Age
- Size
- Sex
- Medical needs
- Behavior
- Rescue capacity
- Bonded pairs and litters

Transport is arranged separately through the shelter's existing network (including airport and pilot partners), after a match is found.

## What It Does

- Combines the partners' different spreadsheet formats into one consistent set of fields
- Turns loosely written intake notes into criteria that can be filtered
- Handles individual animals, bonded pairs, and litters
- Shows which rescues an animal qualifies for, based on clear rules, so staff can see why each match was made

## How AI Was Used

I used AI tools during development to:

- Help design the data structure
- Standardize inconsistent terms across partner spreadsheets
- Sort loosely written intake notes into consistent categories
- Build and revise prototypes quickly

Placement decisions are always made by shelter staff, not the tool.

## How It's Built

The tool runs locally as a single HTML/JavaScript file with the data built in. I chose this so that:

- It needs no servers, accounts, or internet connection
- Shelter and partner data stay on the shelter's own computer
- It's simple to set up and keep running with limited IT support

The matching follows fixed rules, so the same input always gives the same result.

## Tradeoffs

| Choice | Benefit | Cost |
|---|---|---|
| Runs locally | Simple, private, no infrastructure | Can't be shared across locations easily |
| Fixed-rule matching | Transparent and easy to check | Doesn't learn or rank by likely success |
| Modeling pairs and litters | Fewer matches that fall apart later | More setup work up front |

## Data & Privacy

This repository contains documentation only. It does not include shelter spreadsheets, partner criteria, transport lists, or any other sensitive information.

## Contact

For more detail or a sanitized demo, reach out through GitHub or LinkedIn.
