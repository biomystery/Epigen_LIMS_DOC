# FAQs

## Library name convention

1. Named using `initials_nth`: e.g.: `JYH_123` 

## Seq name convention

Because each sequencing is derivated from a library, the sequence id
need match with the library's id. By default, we thought the library
is only sequence once, so **always** the first sequencing id is
idential to the library ID (i.e. No `JYH_123_1` for the first
sequencing). Then the next sequencing made from the same library named
as "JYH_123_2" and etc. 

## Pooled libraries
The pooled lirary should be named as `JYH_123_1_2` and etc. For
`JYH_123_1_2`, it means to pool `JYH_123` and `JYH_123_2` togather. If
you want to pool `JYH_123` and `JYH_123_3` togather, then the name
should be `JYH_123_1_3`. 

## Collaborator Validation (through sample creation interface)
While you create new samples, the app will extract the collaborators' profile from column B-H, then do some viladations on these and link the samples with collaborators in the meantime.
Basically, the validation rule is that the group name, research contact name, email, phone, fiscal contact’s name, email as well as the index should exactly match with the database. If you are not sure about this, you could go to [Collaborators Table](http://epigenomics.sdsc.edu:8000/manager/collab_list/) to check.
If they have passed the validations, you would see the extra columns of  ‘group’,’research_person’  and ‘ fiscal_person_index’ in the Preview page:


If not, the app would report an error and you could not save the samples into database. 
The error message would tell you what is wrong and instruct you how you can fix them, like an example shows below. In this example, the group name is misspelled:



