# Write-a-trigger-OR-CREATE-A-_start-date_-and-_end-date-fiels_-and-also-creste-_active-true-false-_-f
Write a trigger OR CREATE A _start date_ and _end date fiels_ and also creste _active(true/false)_ field on Opportunity object if Current date in between start/end date then  is avtive field must be true 
pubic static void isActive(list<opportunity> oppnewlist)


for(Opportunity opp:oppnewlist)
{

   if(opp.StartDate__c<=system.today()  && opp.EndDate__c>= system.today())
{
    opp.Active__c=true;
    
}
}
