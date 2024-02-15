Ghostly privileged - Tale of Transitive privileges on Azure

In today’s complex IT environments, it’s not enough to simply limit access to resources. Transitive relationships between resources can create hairline vulnerabilities that can be exploited by attackers. That’s why we propose to share the importance of access check relationships inside Azure services and demonstrate how we can use them to proactively detect potential security vulnerabilities. For instance, user A has access to a VM [MSI] and this MSI has access to a Keyvault. It’s hard to identify that User A has access to Keyvault (or any other resource). However, if not properly managed, they can create unintended access paths and increase the risk of privilege escalation attacks. We’ll show how to use already present data to identify and manage these relationships to reduce the risk of security breaches. The notebook that will be presented can be used to identify transitive relationships that end up being high privileged. This is done using Graph (python network graphing module), pandas (for data structuring), Azure API (for fetching data).![image](https://github.com/PallaviKumariJha/Notebooks/assets/2514003/fb774052-04e7-4ef2-8afd-49bf15ec8f53)
