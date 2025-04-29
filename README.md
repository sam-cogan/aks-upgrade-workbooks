# AKS Upgrade Workbooks

This repository contains Azure Monitor workbooks designed to help Azure Kubernetes Service (AKS) administrators monitor and manage cluster version upgrades.

## Workbooks

### 1. aks-upgrade-workbook.json

This workbook provides an overview of Kubernetes versions and helps you identify clusters that need to be upgraded. It offers:

- A list of currently supported Kubernetes versions with their support plans:
  - KubernetesOfficial: standard releases, supported for one year
  - AKSLongTermSupport: Long Term Support releases, supported for 2 years
- Identification of clusters running versions older than a selected version
- Visibility into which clusters need upgrades to stay on supported versions

### 2. aks-upgrades-for-cluster.json

This workbook provides detailed information about specific AKS clusters and available upgrade paths:

- Lists all AKS clusters with their current Kubernetes version
- Shows available upgrade versions for a selected cluster
- Helps plan and track cluster upgrade operations

## How to Use

1. Import these workbooks into your Azure Portal by:
   - Going to Azure Monitor
   - Selecting "Workbooks"
   - Clicking "New" or "Open"
   - Selecting "Gallery Template" 
   - Clicking "Import" and selecting the workbook JSON file
   - Update any subscription and resource group values to reflect your own environment

2. Once imported, these workbooks will help you:
   - Identify which clusters need version upgrades
   - Determine available upgrade paths for specific clusters
   - Plan your AKS upgrade strategy

## Requirements

- Azure subscription with AKS clusters
- Appropriate permissions to access resources via Azure Resource Graph
- Azure Portal access

## Purpose

These workbooks are designed to simplify the process of keeping your AKS clusters up-to-date with the latest Kubernetes versions, helping maintain security, stability, and access to new features.