# Amazon Elastic Compute Cloud User Guide for Linux Instances

-----
*****Copyright &copy; Amazon Web Services, Inc. and/or its affiliates. All rights reserved.*****

-----
Amazon's trademarks and trade dress may not be used in 
     connection with any product or service that is not Amazon's, 
     in any manner that is likely to cause confusion among customers, 
     or in any manner that disparages or discredits Amazon. All other 
     trademarks not owned by Amazon are the property of their respective
     owners, who may or may not be affiliated with, connected to, or 
     sponsored by Amazon.

-----
## Contents
+ [What is Amazon EC2?](concepts.md)
+ [Set up to use Amazon EC2](get-set-up-for-amazon-ec2.md)
+ [Tutorial: Get started with Amazon EC2 Linux instances](EC2_GetStarted.md)
+ [Best practices for Amazon EC2](ec2-best-practices.md)
+ [Tutorials for Amazon EC2 Instances Running Linux](ec2-tutorials.md)
   + [Tutorial: Install a LAMP web server on Amazon Linux 2022](ec2-lamp-amazon-linux-2022.md)
   + [Tutorial: Install a LAMP web server on Amazon Linux 2](ec2-lamp-amazon-linux-2.md)
   + [Tutorial: Install a LAMP web server on the Amazon Linux AMI](install-LAMP.md)
   + [Tutorial: Configure SSL/TLS on Amazon Linux 2022](SSL-on-amazon-linux-2022.md)
   + [Tutorial: Configure SSL/TLS on Amazon Linux 2](SSL-on-amazon-linux-2.md)
   + [Tutorial: Configure SSL/TLS with the Amazon Linux AMI](SSL-on-amazon-linux-ami.md)
   + [Tutorial: Host a WordPress blog on Amazon Linux 2022](hosting-wordpress-aml-2022.md)
   + [Tutorial: Host a WordPress blog on Amazon Linux 2](hosting-wordpress.md)
+ [Amazon Machine Images (AMI)](AMIs.md)
   + [AMI types](ComponentsAMIs.md)
   + [Linux AMI virtualization types](virtualization_types.md)
   + [Boot modes](ami-boot.md)
   + [Find a Linux AMI](finding-an-ami.md)
   + [Shared AMIs](sharing-amis.md)
      + [Find shared AMIs](usingsharedamis-finding.md)
      + [Make an AMI public](sharingamis-intro.md)
      + [Share an AMI with specific organizations or organizational units](share-amis-with-organizations-and-OUs.md)
      + [Share an AMI with specific AWS accounts](sharingamis-explicit.md)
      + [Use bookmarks](using-bookmarks.md)
      + [Guidelines for shared Linux AMIs](building-shared-amis.md)
   + [Paid AMIs](paid-amis.md)
   + [AMI lifecycle](ami-lifecycle.md)
      + [Create an AMI](create-ami.md)
         + [Create an Amazon EBS-backed Linux AMI](creating-an-ami-ebs.md)
         + [Create an instance store-backed Linux AMI](creating-an-ami-instance-store.md)
            + [Set up the AMI tools](set-up-ami-tools.md)
            + [Create an AMI from an instance store-backed instance](create-instance-store-ami.md)
            + [Convert your instance store-backed AMI to an Amazon EBS-backed AMI](Using_ConvertingS3toEBS.md)
            + [AMI tools reference](ami-tools-commands.md)
      + [Copy an AMI](CopyingAMIs.md)
      + [Store and restore an AMI using S3](ami-store-restore.md)
      + [Deprecate an AMI](ami-deprecate.md)
      + [Deregister your AMI](deregister-ami.md)
      + [Recover AMIs from the Recycle Bin](recycle-bin-working-with-amis.md)
      + [Automate the EBS-backed AMI lifecycle](automating-amis.md)
   + [Use encryption with EBS-backed AMIs](AMIEncryption.md)
   + [Understand AMI billing information](ami-billing-info.md)
      + [AMI billing information fields](billing-info-fields.md)
      + [Finding AMI billing and usage details](view-billing-info.md)
      + [Verify AMI charges on your bill](verify-ami-charges.md)
   + [Amazon Linux](amazon-linux-ami-basics.md)
      + [Run Amazon Linux 2 as a virtual machine on premises](amazon-linux-2-virtual-machine.md)
      + [Kernel Live Patching on Amazon Linux 2](al2-live-patching.md)
   + [User provided kernels](UserProvidedKernels.md)
   + [Configure the Amazon Linux 2 MATE desktop connection](amazon-linux-ami-mate.md)
+ [Amazon EC2 instances](Instances.md)
   + [Instances and AMIs](ec2-instances-and-amis.md)
   + [Instance types](instance-types.md)
      + [General purpose instances](general-purpose-instances.md)
         + [Burstable performance instances](burstable-performance-instances.md)
            + [Key concepts and definitions for burstable performance instances](burstable-credits-baseline-concepts.md)
            + [Unlimited mode for burstable performance instances](burstable-performance-instances-unlimited-mode.md)
               + [Unlimited mode concepts](burstable-performance-instances-unlimited-mode-concepts.md)
               + [Unlimited mode examples](unlimited-mode-examples.md)
            + [Standard mode for burstable performance instances](burstable-performance-instances-standard-mode.md)
               + [Standard mode concepts](burstable-performance-instances-standard-mode-concepts.md)
               + [Standard mode examples](standard-mode-examples.md)
            + [Work with burstable performance instances](burstable-performance-instances-how-to.md)
            + [Monitor your CPU credits for burstable performance instances](burstable-performance-instances-monitoring-cpu-credits.md)
      + [Compute optimized instances](compute-optimized-instances.md)
      + [Memory optimized instances](memory-optimized-instances.md)
      + [Storage optimized instances](storage-optimized-instances.md)
      + [Linux accelerated computing instances](accelerated-computing-instances.md)
         + [Install NVIDIA drivers on Linux instances](install-nvidia-driver.md)
         + [Install AMD drivers on Linux instances](install-amd-driver.md)
         + [Activate NVIDIA GRID Virtual Applications](activate_grid.md)
         + [Optimize GPU settings](optimize_gpu.md)
      + [Find an Amazon EC2 instance type](instance-discovery.md)
      + [Get recommendations for an instance type](ec2-instance-recommendations.md)
      + [Change the instance type](ec2-instance-resize.md)
         + [Compatibility for changing the instance type](resize-limitations.md)
         + [Troubleshoot changing the instance type](troubleshoot-change-instance-type.md)
         + [Change the instance type of an instance store-backed instance](resize-instance-store-backed-instance.md)
   + [Amazon EC2 Mac instances](ec2-mac-instances.md)
   + [Instance purchasing options](instance-purchasing-options.md)
      + [On-Demand Instances](ec2-on-demand-instances.md)
      + [Reserved Instances](ec2-reserved-instances.md)
         + [Regional and zonal Reserved Instances (scope)](reserved-instances-scope.md)
         + [Types of Reserved Instances (offering classes)](reserved-instances-types.md)
         + [How Reserved Instances are applied](apply_ri.md)
         + [Use your Reserved Instances](using-reserved-instances.md)
         + [How you are billed](concepts-reserved-instances-application.md)
         + [Buy Reserved Instances](ri-market-concepts-buying.md)
         + [Sell in the Reserved Instance Marketplace](ri-market-general.md)
         + [Modify Reserved Instances](ri-modifying.md)
         + [Exchange Convertible Reserved Instances](ri-convertible-exchange.md)
         + [Reserved Instance quotas](ri-limits.md)
      + [Scheduled Reserved Instances](ec2-scheduled-instances.md)
      + [Spot Instances](using-spot-instances.md)
         + [Best practices for EC2 Spot](spot-best-practices.md)
         + [How Spot Instances work](how-spot-instances-work.md)
         + [Spot Instance pricing history](using-spot-instances-history.md)
         + [Savings from purchasing Spot Instances](spot-savings.md)
         + [Spot Instance requests](spot-requests.md)
            + [Spot Instance request example launch specifications](spot-request-examples.md)
         + [Spot request status](spot-request-status.md)
         + [EC2 instance rebalance recommendations](rebalance-recommendations.md)
         + [Spot Instance interruptions](spot-interruptions.md)
            + [Reasons for interruption](interruption-reasons.md)
            + [Interruption behavior](interruption-behavior.md)
            + [Stop interrupted Spot Instances](stop-spot-instances.md)
            + [Hibernate interrupted Spot Instances](hibernate-spot-instances.md)
            + [Terminate interrupted Spot Instances](terminate-interrupted-spot-instances.md)
            + [Prepare for interruptions](prepare-for-interruptions.md)
            + [Spot Instance interruption notices](spot-instance-termination-notices.md)
            + [Find interrupted Spot Instances](finding-an-interrupted-Spot-Instance.md)
            + [Determine whether Amazon EC2 interrupted a Spot Instance](BidEvictedEvent.md)
            + [Billing for interrupted Spot Instances](billing-for-interrupted-spot-instances.md)
         + [Spot placement score](spot-placement-score.md)
         + [Spot Instance data feed](spot-data-feeds.md)
         + [Spot Instance limits](using-spot-limits.md)
         + [Burstable performance instances](burstable-spot-instances.md)
      + [Dedicated Hosts](dedicated-hosts-overview.md)
         + [Work with Dedicated Hosts](how-dedicated-hosts-work.md)
         + [Work with shared Dedicated Hosts](dh-sharing.md)
         + [Host recovery](dedicated-hosts-recovery.md)
         + [Track configuration changes](dedicated-hosts-aws-config.md)
      + [Dedicated Instances](dedicated-instance.md)
         + [Work with Dedicated Instances](dedicated-usage-overview.md)
      + [On-Demand Capacity Reservations](ec2-capacity-reservations.md)
         + [Capacity Reservation pricing and billing](capacity-reservations-pricing-billing.md)
         + [Work with Capacity Reservations](capacity-reservations-using.md)
         + [Work with Capacity Reservation groups](create-cr-group.md)
         + [Capacity Reservations in cluster placement groups](cr-cpg.md)
         + [Capacity Reservations in Local Zones](capacity-reservations-localzones.md)
         + [Capacity Reservations in Wavelength Zones](capacity-reservations-wavelengthzones.md)
         + [Capacity Reservations on AWS Outposts](capacity-reservations-outposts.md)
         + [Work with shared Capacity Reservations](capacity-reservation-sharing.md)
         + [Capacity Reservation Fleets](cr-fleets.md)
            + [Capacity Reservation Fleet concepts](crfleet-concepts.md)
            + [Work with Capacity Reservation Fleets](work-with-cr-fleets.md)
            + [Example Capacity Reservation Fleet configurations](example-configs.md)
            + [Using Service-Linked Roles for Capacity Reservation Fleet](using-service-linked-roles.md)
         + [CloudWatch metrics for On-Demand Capacity Reservations](capacity-reservation-cw-metrics.md)
   + [Instance lifecycle](ec2-instance-lifecycle.md)
      + [Launch your instance](LaunchingAndUsingInstances.md)
         + [Launch an instance using the new launch instance wizard](ec2-launch-instance-wizard.md)
            + [Launch an instance using the old launch instance wizard](launching-instance.md)
         + [Launch an instance from a launch template](ec2-launch-templates.md)
         + [Launch an instance using parameters from an existing instance](launch-more-like-this.md)
         + [Launch an AWS Marketplace instance](launch-marketplace-console.md)
      + [Connect to your Linux instance](AccessingInstances.md)
         + [General prerequisites for connecting to your instance](connection-prereqs.md)
         + [Connect to your Linux instance using SSH](AccessingInstancesLinux.md)
         + [Connect to your Linux instance using EC2 Instance Connect](Connect-using-EC2-Instance-Connect.md)
            + [Set up EC2 Instance Connect](ec2-instance-connect-set-up.md)
            + [Connect using EC2 Instance Connect](ec2-instance-connect-methods.md)
            + [Uninstall EC2 Instance Connect](ec2-instance-connect-uninstall.md)
         + [Connect to your Linux instance from Windows using PuTTY](putty.md)
         + [Connect to your Linux instance from Windows using Windows Subsystem for Linux](WSL.md)
         + [Connect to your Linux instance using Session Manager](session-manager.md)
      + [Stop and start your instance](Stop_Start.md)
      + [Hibernate your On-Demand Linux instance](Hibernate.md)
         + [Overview of hibernation](instance-hibernate-overview.md)
         + [Hibernation prerequisites](hibernating-prerequisites.md)
         + [Limitations](instance-hibernate-limitations.md)
         + [Configure an existing AMI to support hibernation](hibernation-enabled-AMI.md)
         + [Enable hibernation for an instance](enabling-hibernation.md)
         + [Disable KASLR on an instance (Ubuntu only)](hibernation-disable-kaslr.md)
         + [Hibernate an instance](hibernating-instances.md)
         + [Start a hibernated instance](hibernating-resuming.md)
         + [Troubleshoot hibernation](troubleshoot-instance-hibernate.md)
      + [Reboot your instance](ec2-instance-reboot.md)
      + [Instance retirement](instance-retirement.md)
      + [Terminate your instance](terminating-instances.md)
      + [Recover your instance](ec2-instance-recover.md)
   + [Configure your Amazon Linux instance](Configure_Instance.md)
      + [Manage software on your Amazon Linux instance](managing-software.md)
         + [Update instance software on your Amazon Linux instance](install-updates.md)
         + [Add repositories on an Amazon Linux instance](add-repositories.md)
         + [Find software packages on an Amazon Linux instance](find-software.md)
         + [Install software packages on an Amazon Linux instance](install-software.md)
         + [Prepare to compile software on an Amazon Linux instance](compile-software.md)
      + [Manage user accounts on your Amazon Linux instance](managing-users.md)
      + [Processor state control for your EC2 instance](processor_state_control.md)
      + [I/O scheduler](io-scheduler.md)
      + [Set the time for your Linux instance](set-time.md)
      + [Optimize CPU options](instance-optimize-cpu.md)
         + [Rules for specifying CPU options](instance-cpu-options-rules.md)
         + [CPU cores and threads per CPU core per instance type](cpu-options-supported-instances-values.md)
         + [Specify CPU options for your instance](instance-specify-cpu-options.md)
         + [View the CPU options for your instance](view-cpu-options.md)
      + [Change the hostname of your Amazon Linux instance](set-hostname.md)
      + [Set up dynamic DNS on Your Amazon Linux instance](dynamic-dns.md)
      + [Run commands on your Linux instance at launch](user-data.md)
      + [Instance metadata and user data](ec2-instance-metadata.md)
         + [Use IMDSv2](configuring-instance-metadata-service.md)
         + [Configure the instance metadata options](configuring-instance-metadata-options.md)
         + [Retrieve instance metadata](instancedata-data-retrieval.md)
         + [Work with instance user data](instancedata-add-user-data.md)
         + [Retrieve dynamic data](instancedata-dynamic-data-retrieval.md)
         + [Instance metadata categories](instancedata-data-categories.md)
         + [Example: AMI launch index value](AMI-launch-index-examples.md)
         + [Instance identity documents](instance-identity-documents.md)
            + [Use the PKCS7 signature to verify the instance identity document](verify-pkcs7.md)
            + [Use the base64-encoded signature to verify the instance identity document](verify-signature.md)
            + [Use the RSA-2048 signature to verify the instance identity document](verify-rsa2048.md)
   + [Amazon Elastic Inference](elastic-inference.md)
   + [Identify EC2 Linux instances](identify_ec2_instances.md)
+ [EC2 Fleet and Spot Fleet](Fleets.md)
   + [EC2 Fleet](ec2-fleet.md)
      + [EC2 Fleet request types](ec2-fleet-request-type.md)
         + [Use an EC2 Fleet of type 'instant'](instant-fleet.md)
      + [EC2 Fleet configuration strategies](ec2-fleet-configuration-strategies.md)
         + [Plan an EC2 Fleet](plan-ec2-fleet.md)
         + [Allocation strategies for Spot Instances](ec2-fleet-allocation-strategy.md)
         + [Attribute-based instance type selection for EC2 Fleet](ec2-fleet-attribute-based-instance-type-selection.md)
         + [Configure EC2 Fleet for On-Demand backup](ec2-fleet-on-demand-backup.md)
         + [Capacity Rebalancing](ec2-fleet-capacity-rebalance.md)
         + [Maximum price overrides](ec2-fleet-price-overrides.md)
         + [Control spending](ec2-fleet-control-spending.md)
         + [EC2 Fleet instance weighting](ec2-fleet-instance-weighting.md)
      + [Work with EC2 Fleets](manage-ec2-fleet.md)
   + [Spot Fleet](spot-fleet.md)
      + [Spot Fleet request types](spot-fleet-requests.md)
      + [Spot Fleet configuration strategies](how-spot-fleet-works.md)
         + [Plan a Spot Fleet request](plan-spot-fleet.md)
         + [Allocation strategy for Spot Instances](spot-fleet-allocation-strategy.md)
         + [Attribute-based instance type selection for Spot Fleet](spot-fleet-attribute-based-instance-type-selection.md)
         + [On-Demand in Spot Fleet](on-demand-in-spot.md)
         + [Capacity Rebalancing](spot-fleet-capacity-rebalance.md)
         + [Spot price overrides](spot-price-overrides.md)
         + [Control spending](spot-fleet-control-spending.md)
         + [Spot Fleet instance weighting](spot-instance-weighting.md)
      + [Work with Spot Fleets](work-with-spot-fleets.md)
      + [CloudWatch metrics for Spot Fleet](spot-fleet-cloudwatch-metrics.md)
      + [Automatic scaling for Spot Fleet](spot-fleet-automatic-scaling.md)
         + [Scale Spot Fleet using a target tracking policy](spot-fleet-target-tracking.md)
         + [Scale Spot Fleet using step scaling policies](spot-fleet-step-scaling.md)
         + [Scale Spot Fleet using scheduled scaling](spot-fleet-scheduled-scaling.md)
   + [Monitor fleet events using Amazon EventBridge](fleet-monitor.md)
      + [EC2 Fleet event types](ec2-fleet-event-types.md)
      + [Spot Fleet event types](spot-fleet-event-types.md)
      + [Create Amazon EventBridge rules](fleet_create-eventbridge-rules.md)
         + [Create Amazon EventBridge rules to monitor EC2 Fleet events](ec2-fleet-using-eventbridge.md)
         + [Create Amazon EventBridge rules to monitor Spot Fleet events](spot-fleet-using-eventbridge.md)
   + [Tutorials for EC2 Fleet and Spot Fleet](fleet-tutorials.md)
      + [Tutorial: Use EC2 Fleet with instance weighting](ec2-fleet-instance-weighting-walkthrough.md)
      + [Tutorial: Use EC2 Fleet with On-Demand as the primary capacity](ec2-fleet-on-demand-walkthrough.md)
      + [Tutorial: Launch On-Demand Instances using targeted Capacity Reservations](ec2-fleet-launch-on-demand-instances-using-targeted-capacity-reservations-walkthrough.md)
      + [Tutorial: Use Spot Fleet with instance weighting](instance-weighting-walkthrough.md)
   + [Example configurations for EC2 Fleet and Spot Fleet](fleet-examples.md)
      + [EC2 Fleet example configurations](ec2-fleet-examples.md)
      + [Spot Fleet example configurations](spot-fleet-examples.md)
   + [Fleet quotas](fleet-quotas.md)
+ [Monitor Amazon EC2](monitoring_ec2.md)
   + [Automated and manual monitoring](monitoring_automated_manual.md)
   + [Best practices for monitoring](monitoring_best_practices.md)
   + [Monitor the status of your instances](monitoring-instances-status-check.md)
      + [Status checks for your instances](monitoring-system-instance-status-check.md)
      + [Scheduled events for your instances](monitoring-instances-status-check_sched.md)
         + [Define event windows for scheduled events](event-windows.md)
   + [Monitor your instances using CloudWatch](using-cloudwatch.md)
      + [Enable or turn off detailed monitoring for your instances](using-cloudwatch-new.md)
      + [List the available CloudWatch metrics for your instances](viewing_metrics_with_cloudwatch.md)
      + [Get statistics for metrics for your instances](monitoring_get_statistics.md)
         + [Get statistics for a specific instance](US_SingleMetricPerInstance.md)
         + [Aggregate statistics across instances](GetSingleMetricAllDimensions.md)
         + [Aggregate statistics by Auto Scaling group](GetMetricAutoScalingGroup.md)
         + [Aggregate statistics by AMI](US_SingleMetricPerAMI.md)
      + [Graph metrics for your instances](graphs-in-the-aws-management-console.md)
      + [Create a CloudWatch alarm for an instance](using-cloudwatch-createalarm.md)
      + [Create alarms that stop, terminate, reboot, or recover an instance](UsingAlarmActions.md)
   + [Automate Amazon EC2 with EventBridge](automating_with_eventbridge.md)
   + [Monitor memory and disk metrics for Amazon EC2 Linux instances](mon-scripts.md)
      + [Deprecated: Collect metrics using the CloudWatch monitoring scripts](monitoring-scripts-intro.md)
   + [Log Amazon EC2 and Amazon EBS API calls with AWS CloudTrail](monitor-with-cloudtrail.md)
+ [Networking in Amazon EC2](ec2-networking.md)
   + [Regions and Zones](using-regions-availability-zones.md)
   + [Amazon EC2 instance IP addressing](using-instance-addressing.md)
      + [Multiple IP addresses](MultipleIP.md)
   + [Amazon EC2 instance hostname types](ec2-instance-naming.md)
   + [Bring your own IP addresses (BYOIP) in Amazon EC2](ec2-byoip.md)
   + [Assigning prefixes to Amazon EC2 network interfaces](ec2-prefix-eni.md)
      + [Work with prefixes](work-with-prefixes.md)
   + [Elastic IP addresses](elastic-ip-addresses-eip.md)
   + [Elastic network interfaces](using-eni.md)
      + [Best practices for configuring network interfaces](best-practices-for-configuring-network-interfaces.md)
      + [Scenarios for network interfaces](scenarios-enis.md)
      + [Requester-managed network interfaces](requester-managed-eni.md)
   + [Amazon EC2 instance network bandwidth](ec2-instance-network-bandwidth.md)
   + [Enhanced networking on Linux](enhanced-networking.md)
      + [Enable enhanced networking with the Elastic Network Adapter (ENA) on Linux instances](enhanced-networking-ena.md)
      + [Enable enhanced networking with the Intel 82599 VF interface on Linux instances](sriov-networking.md)
      + [Operating system optimizations](enhanced-networking-os.md)
      + [Monitor network performance for your EC2 instance](monitoring-network-performance-ena.md)
      + [Troubleshoot the Elastic Network Adapter (ENA)](troubleshooting-ena.md)
   + [Elastic Fabric Adapter](efa.md)
      + [Get started with EFA and MPI](efa-start.md)
      + [Get started with EFA and NCCL](efa-start-nccl.md)
         + [Use a base AMI](efa-start-nccl-base.md)
         + [Use an AWS Deep Learning AMI](efa-start-nccl-dlami.md)
      + [Work with EFA](efa-working-with.md)
      + [Monitor an EFA](efa-working-monitor.md)
      + [Verify the EFA installer using a checksum](efa-verify.md)
   + [Placement groups](placement-groups.md)
   + [Network maximum transmission unit (MTU) for your EC2 instance](network_mtu.md)
   + [Virtual private clouds](using-vpc.md)
   + [EC2-Classic](ec2-classic-platform.md)
      + [ClassicLink](vpc-classiclink.md)
      + [Migrate from EC2-Classic to a VPC](vpc-migrate.md)
+ [Security in Amazon EC2](ec2-security.md)
   + [Infrastructure security in Amazon EC2](infrastructure-security.md)
   + [Resilience in Amazon EC2](disaster-recovery-resiliency.md)
   + [Data protection in Amazon EC2](data-protection.md)
   + [Identity and access management for Amazon EC2](security-iam.md)
      + [IAM policies for Amazon EC2](iam-policies-for-amazon-ec2.md)
         + [Policy structure](iam-policy-structure.md)
         + [Grant permission to tag resources during creation](supported-iam-actions-tagging.md)
         + [Control access to EC2 resources using resource tags](control-access-with-tags.md)
         + [Example policies for working with the AWS CLI or an AWS SDK](ExamplePolicies_EC2.md)
         + [Example policies for working in the Amazon EC2 console](iam-policies-ec2-console.md)
      + [AWS managed policies for Amazon Elastic Compute Cloud](security-iam-awsmanpol.md)
      + [IAM roles for Amazon EC2](iam-roles-for-amazon-ec2.md)
      + [Authorize inbound traffic for your Linux instances](authorizing-access-to-an-instance.md)
   + [Amazon EC2 key pairs and Linux instances](ec2-key-pairs.md)
      + [Create key pairs](create-key-pairs.md)
      + [Tag a public key](tag-key-pair.md)
      + [Describe public keys](describe-keys.md)
      + [Delete your public key on Amazon EC2](delete-key-pair.md)
      + [Add or remove a public key on your instance](replacing-key-pair.md)
      + [Verify keys](verify-keys.md)
   + [Amazon EC2 security groups for Linux instances](ec2-security-groups.md)
      + [Security group rules](security-group-rules.md)
      + [Security group connection tracking](security-group-connection-tracking.md)
      + [Default and custom security groups](default-custom-security-groups.md)
      + [Work with security groups](working-with-security-groups.md)
      + [Security group rules for different use cases](security-group-rules-reference.md)
   + [Access Amazon EC2 using an interface VPC endpoint](interface-vpc-endpoints.md)
   + [Update management in Amazon EC2](update-management.md)
   + [Compliance validation for Amazon EC2](compliance-validation.md)
+ [Storage](Storage.md)
   + [Amazon Elastic Block Store (Amazon EBS)](AmazonEBS.md)
      + [Amazon EBS volumes](ebs-volumes.md)
         + [Amazon EBS volume types](ebs-volume-types.md)
         + [Constraints on the size and configuration of an EBS volume](volume_constraints.md)
         + [Create an Amazon EBS volume](ebs-creating-volume.md)
         + [Attach an Amazon EBS volume to an instance](ebs-attaching-volume.md)
         + [Attach a volume to multiple instances with Amazon EBS Multi-Attach](ebs-volumes-multi.md)
         + [Make an Amazon EBS volume available for use on Linux](ebs-using-volumes.md)
         + [View information about an Amazon EBS volume](ebs-describing-volumes.md)
         + [Replace an Amazon EBS volume](ebs-restoring-volume.md)
         + [Monitor the status of your volumes](monitoring-volume-status.md)
         + [Detach an Amazon EBS volume from a Linux instance](ebs-detaching-volume.md)
         + [Delete an Amazon EBS volume](ebs-deleting-volume.md)
      + [Amazon EBS snapshots](EBSSnapshots.md)
         + [Create Amazon EBS snapshots](ebs-creating-snapshot.md)
         + [Delete an Amazon EBS snapshot](ebs-deleting-snapshot.md)
         + [Copy an Amazon EBS snapshot](ebs-copy-snapshot.md)
         + [Archive Amazon EBS snapshots](snapshot-archive.md)
            + [Guidelines and best practices for archiving snapshots](archiving-guidelines.md)
            + [Work with snapshot archiving](working-with-snapshot-archiving.md)
            + [Monitor snapshot archiving](monitor-snapshot-archiving.md)
         + [View Amazon EBS snapshot information](ebs-describing-snapshots.md)
         + [Share an Amazon EBS snapshot](ebs-modifying-snapshot-permissions.md)
         + [Recover snapshots from the Recycle Bin](recycle-bin-working-with-snaps.md)
         + [Amazon EBS local snapshots on Outposts](snapshots-outposts.md)
         + [Use EBS direct APIs to access the contents of an EBS snapshot](ebs-accessing-snapshot.md)
            + [IAM permissions for EBS direct APIs](ebsapi-permissions.md)
            + [Use EBS direct APIs](work-with.md)
               + [Read snapshots with EBS direct APIs](readsnapshots.md)
               + [Write snapshots with EBS direct APIs](writesnapshots.md)
               + [Use encryption](ebsapis-using-encryption.md)
               + [Use Signature Version 4 signing](ebsapis-using-sigv4.md)
               + [Use checksums](ebsapis-using-checksums.md)
               + [Idempotency for StartSnapshot API](ebs-direct-api-idempotency.md)
               + [Error retries](error-retries.md)
               + [Optimize performance](ebsapi-performance.md)
            + [Using interface VPC endpoints with EBS direct APIs](ebs-apis-vpc-endpoints.md)
            + [Log API Calls for EBS direct APIs with AWS CloudTrail](logging-ebs-apis-using-cloudtrail.md)
            + [Frequently asked questions](ebsapi-faq.md)
         + [Automate the snapshot lifecycle](automating-snapshots.md)
      + [Amazon Data Lifecycle Manager](snapshot-lifecycle.md)
         + [Automate snapshot lifecycles](snapshot-ami-policy.md)
         + [Automate AMI lifecycles](ami-policy.md)
         + [Automate cross-account snapshot copies](event-policy.md)
         + [View, modify, and delete lifecycle policies](view-modify-delete.md)
         + [AWS Identity and Access Management](dlm-prerequisites.md)
            + [AWS managed policies](managed-policies.md)
            + [IAM service roles](service-role.md)
            + [Permissions for IAM users](dlm-access-control.md)
            + [Permissions for encryption](dlm-access-cmk.md)
         + [Monitor the lifecycle of snapshots and AMIs](dlm-monitor-lifecycle.md)
            + [Monitor your policies using CloudWatch Events](monitor-cloudwatch-events.md)
            + [Monitor your policies using Amazon CloudWatch](monitor-dlm-cw-metrics.md)
      + [Amazon EBS data services](ebs-data-services.md)
         + [Amazon EBS Elastic Volumes](ebs-modify-volume.md)
            + [Requirements when modifying volumes](modify-volume-requirements.md)
            + [Request modifications to your EBS volumes](requesting-ebs-volume-modifications.md)
            + [Monitor the progress of volume modifications](monitoring-volume-modifications.md)
            + [Extend a Linux file system after resizing a volume](recognize-expanded-volume-linux.md)
         + [Amazon EBS encryption](EBSEncryption.md)
         + [Amazon EBS fast snapshot restore](ebs-fast-snapshot-restore.md)
      + [Amazon EBS and NVMe on Linux instances](nvme-ebs-volumes.md)
      + [Amazon EBS–optimized instances](ebs-optimized.md)
      + [Amazon EBS volume performance on Linux instances](EBSPerformance.md)
         + [I/O characteristics and monitoring](ebs-io-characteristics.md)
         + [Initialize Amazon EBS volumes](ebs-initialize.md)
         + [RAID configuration on Linux](raid-config.md)
         + [Benchmark EBS volumes](benchmark_procedures.md)
      + [Amazon CloudWatch metrics for Amazon EBS](using_cloudwatch_ebs.md)
      + [Amazon CloudWatch Events for Amazon EBS](ebs-cloud-watch-events.md)
      + [Amazon EBS quotas](ebs-resource-quotas.md)
   + [Amazon EC2 instance store](InstanceStorage.md)
      + [Add instance store volumes to your EC2 instance](add-instance-store-volumes.md)
      + [SSD instance store volumes](ssd-instance-store.md)
      + [Instance store swap volumes](instance-store-swap-volumes.md)
      + [Optimize disk performance for instance store volumes](disk-performance.md)
   + [File storage](file-storage.md)
      + [Use Amazon S3 with Amazon EC2](AmazonS3.md)
      + [Use Amazon EFS with Amazon EC2](AmazonEFS.md)
      + [Use Amazon FSx with Amazon EC2](storage_fsx.md)
   + [Instance volume limits](volume_limits.md)
   + [Amazon EC2 instance root device volume](RootDeviceStorage.md)
   + [Device names on Linux instances](device_naming.md)
   + [Block device mappings](block-device-mapping-concepts.md)
+ [Resources and tags](EC2_Resources.md)
   + [Recycle Bin](recycle-bin.md)
      + [Considerations](recycle-bin-factors.md)
      + [Required IAM permissions](recycle-bin-perms.md)
      + [Work with retention rules](recycle-bin-working-with-rules.md)
      + [Work with resources in the Recycle Bin](recycle-bin-work-with-resources.md)
      + [Monitoring Recycle Bin using AWS CloudTrail](recycle-bin-ct.md)
   + [Resource locations](resources.md)
   + [Resource IDs](resource-ids.md)
   + [List and filter your resources](Using_Filtering.md)
   + [Tag your Amazon EC2 resources](Using_Tags.md)
   + [Amazon EC2 service quotas](ec2-resource-limits.md)
   + [Amazon EC2 usage reports](usage-reports.md)
+ [Troubleshoot EC2 instances](ec2-instance-troubleshoot.md)
   + [Troubleshoot instance launch issues](troubleshooting-launch.md)
   + [Troubleshoot connecting to your instance](TroubleshootingInstancesConnecting.md)
   + [Troubleshoot stopping your instance](TroubleshootingInstancesStopping.md)
   + [Troubleshoot instance termination (shutting down)](TroubleshootingInstancesShuttingDown.md)
   + [Troubleshoot instances with failed status checks](TroubleshootingInstances.md)
   + [Troubleshoot an unreachable instance](instance-console.md)
   + [Boot from the wrong volume](instance-booting-from-wrong-volume.md)
   + [Use EC2Rescue for Linux](Linux-Server-EC2Rescue.md)
      + [Install EC2Rescue for Linux](ec2rl_install.md)
      + [(Optional) Verify the signature of EC2Rescue for Linux](ec2rl_verify.md)
      + [Work with EC2Rescue for Linux](ec2rl_working.md)
      + [Develop EC2Rescue modules](ec2rl_moduledev.md)
   + [EC2 Serial Console for Linux instances](ec2-serial-console.md)
      + [Configure access to the EC2 Serial Console](configure-access-to-serial-console.md)
      + [Connect to the EC2 Serial Console](connect-to-serial-console.md)
      + [Terminate an EC2 Serial Console session](terminate-serial-console-session.title.md)
      + [Troubleshoot your Linux instance using the EC2 Serial Console](troubleshoot-using-serial-console.md)
         + [Troubleshoot your Linux instance using GRUB](grub.md)
         + [Troubleshoot your Linux instance using SysRq](SysRq.md)
   + [Send a diagnostic interrupt (for advanced users)](diagnostic-interrupt.md)
+ [Document history](DocumentHistory.md)