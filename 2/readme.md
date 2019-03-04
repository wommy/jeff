readme.md
- transpose https://www.hashicorp.com/products/vault/enterprise

h1 vault packages

row 3xCards [open_source, enterprise_pro, enterprise_premium]
	subtitle + img [for_individuals, dot.img]
	h2 [open_source]
	p [Secrets management and data protection]
	button [free, img+download]

hero
	invert bg
	h2 open source vs enterprise
		2xP
		img

compare offering
	row 4xCards
		[img_vault, open_source, enterpise_pro, enterprise_premium]
	table
		header - [secret_management, data_protection, identity-based_access, collab&ops, governance&compliance, multi-datacenter]
		row - [ 100x ]
			title + ? | check | check | check
		footer-row [ download, get_pricing, get_pricing]

table_data:

	secrets management
		dynamic secrets
			[3, Dynamic secrets are generated on demand and are unique to a client and can be revoked immediately after use, minimizing the life of the secret]
		secret storage
			[3, Encrypt data while at rest, in the storage backend of your choice]
		secure plugins
			[3, Improve the extensibility of Vault with pluggable backends]
		detailed audit logs
			[3, Vault stores a detailed audit log of all authenticated client interaction (authentication, token creation, secret access, secret revocation, etc.)]
		leasing & revoking secrets
			[3, Manage authorization tokens throughout your infrastructure: Create time-based tokens for automatic revocation or manual revocation]
		acl templates
			[3, Support templating for identity groups, entities, and metadata within ACL policies]
		vault agent
			[3, Automatically manage the secure introduction and renewal of tokens for local applications]
		init & unseal workflow
			[3, Web browser accessible workflow]
		key rolling
			[3, Key Rolling allows the ability to update and roll new keys throughout distributed infrastructure while retaining the ability to decrypt values encrypted with past key versions]
		ui with cluster management
			[3, Perform all CLI/API actions from one easily accessible browser interface for secret administration and Vault multi-datacenter cluster management]
		entities & identity groups
			[3, An integrated system for understanding the identity of a person or system across their logins and tokens and using this information for policy and access control decisions]
		access control policies
			[3, Create and manage policies that authorize access control throughout your infrastructure and organization]
		identity plugins
			[3, Extend Vault with pluggable authentication methods to directly integrate with your trusted identity providers]

	data protection
		encryption as a service
			[3, Encrypt application data during transit and at rest.]
		transit backend
			[3, Encrypt and decrypt application data with a HTTP (TLS) API call. Key management, encryption algorithm, and more are offloaded and centrally managed by Vault.]
		encryption key rolling
			[3, Encryption key rolling.]

	identity-based access
		entities & identity groups
			[3, An integrated system for understanding the identity of a person or system across their logins and tokens and using this information for policy and access control decisions.]
		access control policies
			[3, Create and manage policies that authorize access control throughout your infrastructure and organization.]
		identity plugins
			[3, Identity plugins.]

	collaboration & operations
		namespaces
			[2, Provide Secure Multi-tenancy within Vault via isolated, self-managed environments.]
		aws kms auto-unseal
			[3, Automatically unseal Vault clusters using AWS Key Management System.]
		azure key vault auto-unseal
			[3, Automatically unseal Vault clusters using Azure Key Vault System.]
		gcp cloud kms auto-unseal
			[3, Automatically unseal Vault clusters using GCP Cloud Key Management System.]

	governance & compliance
		control groups
			[1, Require multiple Identity Entities or members of Identity Groups to authorize an requested action before it is allowed to run.]
		hsm auto-unseal
			[1, Vault integrates HSM Master Key Wrapping and Automatic Unsealing for HSM installations.]
		multi-factor authentication
			[1, Enforce MFA workflows when accessing a secret or a secret path.]
		sentinel integration
			[1, Take advantage of HashiCorp Sentinel to provide extremely flexible access control policies -- even on unauthenticated endpoints.]
		fips 140-2 & seal wrap
			[1, Vault can take advantage of FIPS 140-2-certified HSMs to ensure that Critical Security Parameters are protected in a compliant fashion.]
		read replicas
			[1, Multiply read performance for Vault Enterprise infrastructure via a new type of performance-focused node within Vault to speed up read performance within a single cluster. This is particularly useful for clusters with a high amount of throughput.]

	multi-datacanter
		disacter recovery
			[2, Failover Vault clusters from one data center to another with limited downtime.]
		replication
			[1, Replication provides high availability replication of secrets and policies across multiple data centers and clouds and is built around global deployments of Vault.]
		replication filters
			[1, Selectively whitelist/blacklist and activate or deactivate mounts for Secret Mounts for Replication.]