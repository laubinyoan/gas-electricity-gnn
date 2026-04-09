# GAS-ELECTRICITY-GNN

## MASTER THESIS PROJECT

This repository contains my master's thesis work on **forecasting in coupled gas and electricity systems** using **Machine Learning** models, from **MLP baselines** to **Graph Neural Networks (GNNs)**. :contentReference[oaicite:1]{index=1}

## PROJECT GOAL

The objective is to predict, in a **day-ahead setting**, the next **24 hours** from the previous **72 hours** of data.

The main targets are:
- **p**: electrical production of the **24 GFPPs**,
- **g**: gas injection of the **4 wells**. :contentReference[oaicite:2]{index=2}

## CONTEXT

Gas and electricity systems are strongly coupled through **Gas-Fired Power Plants (GFPPs)**.  
Because of this link, modeling both systems separately may miss important physical information. This project studies whether ML models can better capture this coupling. :contentReference[oaicite:3]{index=3}

## APPROACH

Two main approaches are studied:

### MLP
MLP models are used as a first baseline to:
- validate the data pipeline,
- compare gas-only, electricity-only, and joint inputs,
- analyze the limits of a flat input representation. :contentReference[oaicite:4]{index=4}

### GNN
The GNN approach is designed to better exploit the **network structure** by using:
- **node features**,
- **edge features**,
- and **graph topology**. :contentReference[oaicite:5]{index=5}

## MAIN OBSERVATION

The first results show that predictions are often **too smooth** and do not fully capture rapid variations, especially on aggregated quantities. This suggests that richer architectures and further tuning are needed. :contentReference[oaicite:6]{index=6}

## PERSPECTIVES

Planned improvements include:
- hyperparameter tuning,
- testing other architectures,
- adding more electrical information,
- deeper analysis by node and prediction horizon,
- comparison with other forecasting methods. :contentReference[oaicite:7]{index=7}
