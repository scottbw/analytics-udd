#UDD Entity descriptions
These are draft UDD entity descriptions. Once they have been agreed, they will be transferred to each md file.

#assessment_instance
##Description of assessment_instance entity
An assessment_instance is any learning activity in a module, for which a student receives a grade and/or mark. The assumption is that grades and/or marks in assessment_instances are summative.

#course
##Description of course entity
A course is a learning opportunity that defines a student's learning activities and aim. It is run by an institution and is usually validated to continue over several years with several intakes. A course will usually have a qualification aim.  Example: BA Honours degree in French.

##Notes
The properties of the course entity do not include start date, study mode or location, because the course is at a high level in the UDD structure.  These properties of a learning opportunity are differentiated in the course_instance, student_course_membership and student_on_course_instance entities.

#course_instance
##Description of course_instance entity
A course_instance is a stage of a course with a start date and an end date, often marked by a progression decision point at the end.  Example: a single academic year in a 3 year Honours degree course.

#institution
##Description of institution entity
An institution is the overall provider of one or more courses.  Example: University of Gloucestershire.

#module
##Description of module entity
A module is a self-contained, formally structured unit of study, with a coherent and explicit set of learning outcomes and assessment criteria.

##Notes
This description is the same as the description for the Module entity in the HEDIIP Data Language.

#module_instance
##Description of module_instance entity
A module_instance is the specific offer of a module to students. It therefore has a specific venue and defined assessments.

#module_VLE_map
##Description of module_VLE_map entity
A module_VLE_map links a module in a student record system with module materials in a VLE.

#period
##Description of period entity
A period describes an institution's official start date and end date of a time slice, such as academic year, term and semester that is used in the UDD data.

#staff
##Description of staff entity
A staff element identifies a member of staff at an institution.

#staff_on_course_instance
##Description of staff_on_course_instance entity
A staff_on_course_instance links a member of staff to a course_instance.

#staff_on_mod_instance
##Description of staff_on_mod_instance entity
A staff_on_mod_instance links a member of staff to a module_instance.

#student
##Description of student entity
A student element describes a person undertaking one or more courses.

#student_course_membership
##Description of student_course_membership entity
A student_course_membership describes a student's enrolment on a course.  It is designed to deal with the fact that some students are enrolled on more than one course in their time at an institution.

##Notes
This entity is similar to a HESA Instance element and a HEDIIP Data Language Student Registration entity.

#student_on_a_module_instance
##Description of student_on_a_module_instance entity
A student_on_a_module_instance describes a student's performance on a specific module.

##Notes
This entity is similar to a HESA StudentOnModule element or a HEDIIP Module Instance entity.

#student_on_assessment_instance
##Description of student_on_assessment_instance entity
A student_on_assessment_instance describes a student's performance on a specific assessment.

#student_on_course_instance
##Description of student_on_course_instance entity
A student_on_course_instance describes a student's engagement with a specific stage of a course.

##Notes
This entity has some similarities to a HESA Instance element, but deals with only a single academic year or stage without reference to the whole course, which is covered in student_course_membership.  It is similar to a HEDIIP Data Language Student Course Session entity.