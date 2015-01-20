---
title       : Mortgage Calculator
subtitle    : 
author      : Coursera Student
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]            # {mathjax, quiz, bootstrap}
mode        : selfcontained 
knit        : slidify::knit2slides
---

## What does the App do ?

The App is a simple mortgage calculator. It takes in the following  inputs:

 * Loan Amount: The total loan amount
 * Interest Rate: Annual interest rate
 * Loan term: Loan duration in years

It presents the following results:

 * Monthly installment: the EMI
 * Ammortization schedule for the first 12 months


---

## How is the monthly installment calculated ?

Installment is calculated using the following formula :

    P*R*(1+R^n)/((1+R^n)-1)

Where
    P is the Loan Amount
    R is the interest rate per month
    n is the number of months in the loan period

---

## How is the amortization table displayed ?

 * The amortization table is computed as a data.frame in the server and displayed as a table int he ui.

---

