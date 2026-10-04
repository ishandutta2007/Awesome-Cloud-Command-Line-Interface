# Awesome-Cloud-Command-Line-Interface

# Awesome-Cloud-Command-Line-Interface



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Cloud Management, Infrastructure Automation & Multi-Cloud Operations*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Command-Line Interfaces**. These tools help developers and DevOps engineers manage cloud resources, automate infrastructure, and script multi-cloud workflows directly from the terminal.



**Examples** include Microsoft Azure CLI, AWS CLI, Google Cloud CLI (gcloud), OCI CLI, DigitalOcean CLI (doctl), Linode CLI, IBM Cloud CLI, Vultr CLI, Scaleway CLI, and Alibaba Cloud CLI (the category leaders).



**Open-source emphasis**: Cloud CLIs are **overwhelmingly open-source** — nearly every major cloud provider publishes their CLI under permissive licenses. **AWS CLI v2**, **Azure CLI**, and **Google Cloud CLI** are all actively maintained open-source projects with tens of thousands of GitHub stars. **doctl** (DigitalOcean) is a popular Go-based CLI, while **Linode CLI**, **Vultr CLI**, and **Scaleway CLI** provide full API coverage for smaller providers. This section documents these production-grade solutions.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## 📖 Table of Contents



- [☁️ SaaS/Hosted Platforms](#-saas-hosted-platforms)

- [🔓 Open-Source GitHub Projects](#-open-source-github-projects)

- [🤝 How to Contribute](#-how-to-contribute)

- [⚠️ Disclaimer](#-disclaimer)



## ☁️ SaaS/Hosted Platforms



> **📊 Market Context**: The global cloud CLI market is **not a standalone commercial segment** — CLI tools are **free value-adds** provided by cloud providers to drive platform adoption. The broader cloud infrastructure services market is estimated at **~$1.2T in 2026**, growing at **~18% CAGR**. The CLI layer is **highly concentrated** by cloud provider — AWS, Azure, and GCP each ship their own CLI as the primary programmatic interface. Open-source alternatives like **Pulumi** and **Terraform** (now OpenTofu) compete at the infrastructure-as-code layer above raw CLIs. No CLI holds a "winner-take-all" position; enterprises typically standardize on their primary cloud's CLI plus one IaC tool.



| Platform | Description | Pricing (Starting Tier) | Free Tier Limits | Company Size |

|----------|-------------|------------------------|------------------|--------------|

| **[Microsoft Azure CLI](https://learn.microsoft.com/en-us/cli/azure/)** | Cross-platform CLI for managing Azure resources. Open-source, available on Windows, macOS, Linux, Docker, and Azure Cloud Shell. | **Free** — Azure CLI itself costs nothing. You pay for Azure resources consumed. **Azure free account**: **$200 credit for 30 days** + **12 months of popular free services** . | **Azure free account**: $200 credit (30 days), 55+ always-free services, 12-month free tier for popular services. **Azure Cloud Shell**: Free with 5 GB persistent storage. | **~$281B revenue (Microsoft FY2025)** |

| **[AWS CLI](https://aws.amazon.com/cli/)** | Unified CLI for AWS services. v2 is the current generation with installer-based distribution. Open-source on GitHub. | **Free** — AWS CLI itself costs nothing. **AWS Free Tier**: **$100 sign-up credits** + up to **$100 in additional credits** through activities. **Free plan**: 6 months or until credits exhausted . | **AWS Free Plan**: **6 months free** or until credits exhausted. **Always Free services**: 1M Lambda requests/month, 5GB S3, 750 hours EC2 t2.micro/t3.micro (12 months for new accounts) . | **~$638B revenue (Amazon FY2025)** |

| **[Google Cloud CLI (gcloud)](https://cloud.google.com/sdk/gcloud)** | CLI for Google Cloud. Includes `gcloud`, `gsutil`, and `bq` tools. Free for all Google Cloud users . | **Free** — Cloud SDK is free. **Google Cloud free trial**: **$300 credit for 90 days** . | **Google Cloud Free Tier**: **$300 credit (90 days)** + **20+ always-free products** including 1 e2-micro VM, 5GB Cloud Storage, 1TiB BigQuery queries/month, 2M Cloud Run requests/month . | **~$350B revenue (Alphabet FY2025)** |

| **[OCI CLI](https://docs.oracle.com/en-us/iaas/Content/API/Concepts/cliconcepts.htm)** | Oracle Cloud Infrastructure CLI. Available in Cloud Shell (pre-installed) and as standalone package. | **Free** — OCI CLI itself costs nothing. **Oracle Cloud Free Tier**: **Always Free** resources available indefinitely . | **Oracle Always Free**: 2 Autonomous Databases, 4 Arm Ampere A1 cores + 24GB RAM, 200GB block storage, 20GB object storage, 10TB outbound/month, 1 flexible load balancer . | **~$53B revenue (Oracle FY2025)** |

| **[DigitalOcean CLI (doctl)](https://github.com/digitalocean/doctl)** | Official CLI for DigitalOcean. Go-based, available on macOS, Linux, Windows. | **Free** — doctl itself costs nothing. DigitalOcean services start at **$4/month** (basic droplet). | **$200 credit for 60 days** for new accounts. **No perpetual free tier** for compute . | **Public (DOCN), ~$700M+ revenue** |

| **[Linode CLI](https://www.linode.com/docs/guides/linode-cli/)** | CLI wrapper around Linode API for managing Akamai Cloud Computing resources . | **Free** — CLI is free to all customers . Linode services start at **$5/month** (Nanode). | **$100 credit for 60 days** for new accounts. **No perpetual free tier**. | **Part of Akamai (~$4B+ revenue)** |

| **[IBM Cloud CLI](https://cloud.ibm.com/docs/cli)** | CLI for IBM Cloud. Free tool for administering IBM Cloud from terminal . | **Free** — CLI is free . **IBM Cloud Lite**: Free tier with select services. | **Lite account**: **Never expires** (if created before Oct 25, 2021). **New accounts**: Pay-As-You-Go with **$200 credit for 30 days** . | **~$63B revenue (IBM FY2025)** |

| **[Vultr CLI](https://docs.vultr.com/)** | CLI for managing Vultr cloud infrastructure — instances, networking, storage, and more . | **Free** — CLI is free. Vultr services start at **$2.50/month** (IPv6-only) or **$5/month** (IPv4). | **$100–$300 credit** for new accounts (varies by promotion). **No perpetual free tier** for compute. | **Private (~$500M+ revenue est.)** |

| **[Scaleway CLI](https://github.com/scaleway/scaleway-cli)** | CLI for administering Scaleway accounts and resources. Free tool . | **Free** — CLI is free . Scaleway services start at **€0.0045/hour** (~€3.24/month) for basic instances. | **€100 credit for 30 days** for new accounts. **No perpetual free tier**. | **Private (part of Iliad Group)** |

| **[Alibaba Cloud CLI](https://www.alibabacloud.com/help/en/cli)** | CLI for Alibaba Cloud. Also available via Cloud Shell (web-based) . | **Free** — CLI is free. Alibaba Cloud services start at **$4.50/month** for basic ECS. | **Free trial resources** for new users: compute, storage, database, and AI products. **Eligibility**: verified real-name account, product-level new user, no outstanding balance . | **~$130B revenue (Alibaba FY2025 est.)** |



## 🔓 Open-Source GitHub Projects



Sorted by star count (descending). Star badge links to each repo's stargazers page.



| Repo | Description | Stars |

|---|---|---|

| **[AWS CLI](https://github.com/aws/aws-cli)** — Universal Command Line Interface for Amazon Web Services. v2 is the current generation. Python-based. Apache-2.0. | [![Stars](https://img.shields.io/github/stars/aws/aws-cli?style=social&color=white)](https://github.com/aws/aws-cli/stargazers) | ~16,000 |

| **[Azure CLI](https://github.com/Azure/azure-cli)** — Command-line tools for Azure. Cross-platform, available on Windows, macOS, Linux, Docker, and Cloud Shell. Python-based. MIT. | [![Stars](https://img.shields.io/github/stars/Azure/azure-cli?style=social&color=white)](https://github.com/Azure/azure-cli/stargazers) | ~4,200 |

| **[Google Cloud SDK](https://github.com/google-cloud-sdk/google-cloud-sdk)** — Tools for Google Cloud including gcloud, gsutil, and bq. Available on Linux, macOS, Windows. | [![Stars](https://img.shields.io/github/stars/google-cloud-sdk/google-cloud-sdk?style=social&color=white)](https://github.com/google-cloud-sdk/google-cloud-sdk/stargazers) | ~3,500 |

| **[doctl (DigitalOcean CLI)](https://github.com/digitalocean/doctl)** — Official DigitalOcean CLI. Go-based, available on macOS, Linux, Windows. Apache-2.0. | [![Stars](https://img.shields.io/github/stars/digitalocean/doctl?style=social&color=white)](https://github.com/digitalocean/doctl/stargazers) | ~3,400 |

| **[Scaleway CLI](https://github.com/scaleway/scaleway-cli)** — CLI for Scaleway Cloud. Go-based. Apache-2.0 . | [![Stars](https://img.shields.io/github/stars/scaleway/scaleway-cli?style=social&color=white)](https://github.com/scaleway/scaleway-cli/stargazers) | ~1,100 |

| **[OCI CLI](https://github.com/oracle/oci-cli)** — Oracle Cloud Infrastructure CLI. Python-based. UPL-1.0. | [![Stars](https://img.shields.io/github/stars/oracle/oci-cli?style=social&color=white)](https://github.com/oracle/oci-cli/stargazers) | ~1,000 |

| **[IBM Cloud CLI](https://github.com/IBM-Cloud/ibm-cloud-cli-release)** — IBM Cloud Command Line Interface. Go-based. Apache-2.0 . | [![Stars](https://img.shields.io/github/stars/IBM-Cloud/ibm-cloud-cli-release?style=social&color=white)](https://github.com/IBM-Cloud/ibm-cloud-cli-release/stargazers) | ~200 |

| **[Vultr CLI](https://github.com/vultr/vultr-cli)** — Official Vultr CLI. Go-based. Apache-2.0 . | [![Stars](https://img.shields.io/github/stars/vultr/vultr-cli?style=social&color=white)](https://github.com/vultr/vultr-cli/stargazers) | ~150 |

| **[Alibaba Cloud CLI](https://github.com/aliyun/aliyun-cli)** — Alibaba Cloud CLI. Go-based. Apache-2.0 . | [![Stars](https://img.shields.io/github/stars/aliyun/aliyun-cli?style=social&color=white)](https://github.com/aliyun/aliyun-cli/stargazers) | ~1,000 |

| **[Linode CLI](https://github.com/linode/linode-cli)** — Official Linode CLI. Python-based. Apache-2.0 . | [![Stars](https://img.shields.io/github/stars/linode/linode-cli?style=social&color=white)](https://github.com/linode/linode-cli/stargazers) | ~600 |



**Additional open-source options worth exploring:**



| Repo | Description |

|---|---|

| **[Azure Developer CLI (azd)](https://github.com/Azure/azure-dev)** — Developer-centric CLI for Azure that accelerates provisioning and deployment. MIT. | [![Stars](https://img.shields.io/github/stars/Azure/azure-dev?style=social&color=white)](https://github.com/Azure/azure-dev/stargazers) |

| **[AWS Copilot CLI](https://github.com/aws/copilot-cli)** — CLI for containerized applications on AWS ECS/Fargate. Apache-2.0. | [![Stars](https://img.shields.io/github/stars/aws/copilot-cli?style=social&color=white)](https://github.com/aws/copilot-cli/stargazers) |

| **[Pulumi](https://github.com/pulumi/pulumi)** — Infrastructure as Code in any language. Apache-2.0. | [![Stars](https://img.shields.io/github/stars/pulumi/pulumi?style=social&color=white)](https://github.com/pulumi/pulumi/stargazers) |



## 🤝 How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## ⚠️ Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Cloud CLIs handle sensitive credentials and API keys; ensure proper secret management, least-privilege access, and compliance with organizational security policies.

- **Open-source reality**: Cloud CLIs are **overwhelmingly open-source** — AWS CLI, Azure CLI, Google Cloud SDK, doctl, OCI CLI, IBM Cloud CLI, Vultr CLI, Scaleway CLI, Alibaba Cloud CLI, and Linode CLI are all **free, open-source tools** published by their respective cloud providers. The "SaaS" and "Open-Source" distinction in this list is therefore **semantic** — the SaaS entry refers to the commercial cloud platform the CLI manages, while the Open-Source entry refers to the CLI tool itself. **Every major cloud CLI is free to download, use, and modify** — you pay only for the cloud resources you consume. The open-source path is **universally viable** for cloud CLI tooling.

- **Pricing caveat**: All free tier figures above are **verified against cited search results** but may change without notice. Cloud provider free tiers often have eligibility restrictions (new accounts only), time limits, and service-specific quotas. Always check the provider's official free tier page for current terms.



---



**Made for DevOps engineers, cloud architects, platform teams, and infrastructure developers.**

Let's make cloud command-line interfaces more open, transparent, and accessible.
