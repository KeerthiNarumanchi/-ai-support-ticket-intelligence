# Dataset Documentation

## Dataset

Hugging Face: `Prady06/customer-support-tickets`

## Purpose

This dataset will be used to build a customer support ticket intelligence system.

The initial model will predict the support queue or category from the ticket subject and body.

## Initial Columns

- `subject`: Short summary of the issue
- `body`: Detailed ticket description
- `queue`: Support queue or ticket category
- `priority`: Ticket priority
- `type`: Type of support request
- `language`: Language of the ticket

## Initial Prediction Target

`queue`

## Input Features

The first model will combine:

- `subject`
- `body`

These fields will be combined into one text column called `ticket_text`.

## Future Targets

- `priority`
- `type`

## Planned Data Preparation

- Remove rows with missing ticket text
- Remove exact duplicate tickets
- Review class distribution
- Combine subject and body
- Check ticket text length
- Check for rare classes
- Split data into training and test sets using stratification

## Data Source

https://huggingface.co/datasets/Prady06/customer-support-tickets

## Usage Note

The project will use the public dataset only. No employer or confidential data will be included.
