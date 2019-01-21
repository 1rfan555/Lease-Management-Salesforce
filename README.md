# Lease-Management-Salesforce
Inamdar Brokers owns multiple buildings. They lease out units in their buildings to different vendors. Inamdar Brokers now want to manage their business using Salesforce.


# Users

1.Director(System Administrator)

	-Director will add buildings and their units
	-will approve/reject contracts created by coordinator
	-can search contracts by building/vender name

2.Coordinator

	-will add venders into the system
	-create contracts based on bulding and their units
	-will submit for approval
	-approved/rejected alerts should be sent to vender
	
	
# Standard/Custom Objects


	1.Standard Objects:
		-Contact

	2.Custom Objects:
		-Buildings
		-units
		-contract
		

# Profiles
	
	I have used two profiles with license of salesforce.(Coordinator and Director)
	Director will have full access of all objects and tabs while coordinator is restricted at some extent.
	
# Roles

	Coordinator will report to director.
	
# Relationships

	used master-detail and lookup-relationships.
	created roll-up summary to have total cost of building on basis of unit's prices.
	

# VF pages

	created vfpage for adding bulding and their units.
	created vfpage for contract search by vender/building name.
	used slds in vfpage.
	
# Apex classes

	apex class for adding building and their units
	helper class for adding multiple records of units
	controller class for contract search
	
# Triggers

	written trigger for validations on duplications(Total 3) and field update after approval of contract.
	

# Test classes

	covered total 45% code and still working on it.
	
# Email templates

	created email templates for contract created/approved/rejected
	
	
# Approval process

	one approval process for contract approval.
	
	
	
	
	
