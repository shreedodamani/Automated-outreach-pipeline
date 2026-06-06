# Automated-outreach-pipeline
One domain in → similar companies → decision makers → verified emails → personalized outreach. Built with Apollo, Prospeo, Eazyreach, and Brevo.
# Automated Outreach Pipeline

## Overview

This project implements an end-to-end automated outreach pipeline.

Input:

* One company domain

Output:

* Personalized outreach emails sent to decision makers

Pipeline Flow:

1. Apollo.io

   * Find lookalike companies from a seed domain

2. Prospeo

   * Find decision makers (CEO, CTO, Founder, VP)

3. Eazyreach

   * Resolve verified work emails

4. Brevo

   * Send personalized outreach emails

## Features

* End-to-end automation
* Safety checkpoint before email sending
* Retry handling for API rate limits
* Deduplication of contacts
* JSON report generation
* Modular architecture

## Installation

pip install -r requirements.txt

## Environment Setup

Create a .env file using .env.example

## Run

python pipeline.py stripe.com

## Architecture

Seed Domain
↓
Apollo
↓
Prospeo
↓
Eazyreach
↓
Brevo

## Screenshots

See screenshots folder for execution examples.
