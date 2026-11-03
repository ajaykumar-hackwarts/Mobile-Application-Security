# NSR(Nano Score Rule) :-

Apps are given in the form of clusters.

**Clusters :** A group of similar apps.

- Agent reviews the app to see if they share the same malicious behavior or not.
  
- And categorise as Interesting(genuinely dangerous) or a Not-interesting(false alarm).

**Two type of Clusters :**

- Apk cluster : Cluster is formed based on the app name and package name.   

- Code Cluster : Cluster is formed based on the code present inside that. 


We currently reviewing the apk cluster only. 

Review steps :-

1. First check for top_malware_category This will be the primary PHA to start the analysis.

2. Review the evidence in the 3 randomly selected TP samples. If that is not available we should review the unreviewed samples.
   
3. Interesting cluster should target the same PHA behaviour. Reviewer should able to identify the similar pattern or code flow in all the 3 TP reviews otherwise the cluster is not-interesting.

4. If it is interesting proceed with 3 FP and 3 Unreviewed apps.

5. If it all exists next step is to check for nsr viability using the PLX query.

 a. if PLX query catches fewer than 20 PHA mark "No NSR needed, bulk action taken"

 b. Else mark “A new NSR will be created for this cluster”

6. 
