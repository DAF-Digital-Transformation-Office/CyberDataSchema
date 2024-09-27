# V2.0.0

## Summary
- Dissolved the concept of 'Software' and merged under 'System' which now includes both hardware and software concepts. Looking to expand System ReferenceTable in the future to incoperate Next D3f3END (0.17.0) ontological references for higher fidelity identification and improved traciblity to that solution (and it's analyses).
- Added InstanceOf to System which both ties together physical and logical systems into the same model, allows for OOP style inheritance, and permits for duplicate systems in the same model.
- Vulnerabilities and Risks had first major overhaul since inception of Cyber Data Schema that now ties together Susceptibilities and permits for shareable Vulnerabilities and Risks in a enterprise wide context.


## Major changes
- (Table Name Change) VulnerabilitySource -> CyberEvaluation
- (Table Name Change) CriticalitySource -> CriticalityAssessment
- (Table Deletion) Table Verification deleted
- (Table Deletion) Table SoftwareType deleted
- (Table Deletion) Table SoftwareTestingType deleted
- (Table Deletion) Table SoftwareTest deleted
- (Table Deletion) Table Software deleted
- (Table Deletion) Table SeveritySource deleted
- (Table Deletion) Table Severity deleted
- (Table Deletion) Table Opportunity deleted
- (Table Deletion) Table Means deleted
- (Table Deletion) Table LikelihoodValue deleted
- (Table Deletion) Table IntelligenceRatingValue deleted
- (Table Deletion) Table IntelligenceFusion deleted
- (Table Deletion) Table IntelligenceConfidenceValue deleted
- (Table Deletion) Table ImpactValue deleted
- (Table Deletion) Table Criticality deleted
- (Column Deletion) Removed Vulnerability.VulnerabilitySource_ID
- (Column Deletion) Removed Vulnerability.System_ID
- (Column Deletion) Removed Vulnerability.Software_ID
- (Column Deletion) Removed System.ExternalEntity
- (Column Deletion) Removed Risk.Severity_ID
- (Column Deletion) Removed Risk.Opportunity_ID
- (Column Deletion) Removed Risk.Means_ID
- (Column Deletion) Removed Risk.Criticliaty_ID


## Minor Changes
- (Table Add) Add VulnerabilityIntelligence table
- (Table Add) Add RiskImpactedSystem table
- (Table Add) Add RiskImpactedMission table
- (Table Add) Add CyberSusceptibility table
- (Column Add) Vulnerability_ID to VulnerabilityIntelligence table
- (Column Add) Vulnerabilities to Risk table
- (Column Add) UUID to CyberSusceptibility table
- (Column Add) System_ID to RiskImpactedSystem table
- (Column Add) System_ID to CyberSusceptibility table
- (Column Add) Susceptibilities to CyberEvaluation table
- (Column Add) Risk_ID to RiskImpactedSystem table
- (Column Add) Risk_ID to RiskImpactedMission table
- (Column Add) Name to CyberSusceptibility table
- (Column Add) Mission_ID to RiskImpactedMission table
- (Column Add) IntentConfidence to VulnerabilityIntelligence table
- (Column Add) Intent to VulnerabilityIntelligence table
- (Column Add) IntelligenceProduct_ID to VulnerabilityIntelligence table
- (Column Add) InstanceOf to System table
- (Column Add) Impact to RiskImpactedSystem table
- (Column Add) Impact to RiskImpactedMission table
- (Column Add) Description to CyberSusceptibility table
- (Column Add) CyberSusceptibilities to Vulnerability table
- (Column Add) CyberSusceptibilities to CyberEvaluation table
- (Column Add) Criticality to MissionData table
- (Column Add) CapabilityConfidence to VulnerabilityIntelligence table
- (Column Add) Capability to VulnerabilityIntelligence table


## Patches
- (Update Table Description) Updated description System table
- (Update Column Description) Updated description of column Software of System table
- (New Property) Created the NoLessThan property
- (New Property) Created the NoGreaterThan property
- (Column Type Change) Change System.Supplier_ID to a Array(VARCHAR(255))
- (Column Type Change) Change System.Software to a Boolean
