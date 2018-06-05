# Advanced Settings
---
#### Advanced Module List	
###### It indicates what advanced modules used in your course
###### Put the modules's name (with quotation marks) in square brackets, and separates each using comma. 
###### This property only accept the regular json data, please be careful with the usage of comma, colon, quotes
```
advanced_modules:[
	"lti_consumer",
	"library_content"
]
```

---
#### Certificate Name (Long)	
###### Use this setting only when generating PDF certificates. Between quotation marks, enter the long name of the type of certificate that students receive when they complete the course. For instance, "Certificate of Achievement".
###### the $CourseTitle$ is a placeholder of Course Title, code will use the real course title to replace it
###### Notice that the value of this property should be in a pair of quotes

```
cert_name_long:"$CourseTitle$ Certificate"
```

---
#### Certificate Name (Short)	
###### Use this setting only when generating PDF certificates. Between quotation marks, enter the short name of the type of certificate that students receive when they complete the course. For instance, "Certificate".
###### the $CourseTitle$ is a placeholder of Course Title, code will use the real course title to replace it
###### Notice that the value of this property should be in a pair of quotes
```
cert_name_short:"$CourseTitle$ Certificate"
```
---
#### Certificate Web/HTML View Enabled	
###### It indicates if Web/HTML views are enabled for the course or not
###### The allowed values is: true or false
###### Notice that the value of this property should be in a pair of quotes
```
cert_html_view_enabled:true
```
---
#### Certificates Display Behavior	
###### Use 'end', 'early_with_info', or 'early_no_info'. After certificate generation, students who passed see a link to their certificates on the dashboard and students who did not pass see information about the grading configuration. The default is end, which displays this certificate information to all students after the course end date. To display this certificate information to all students as soon as certificates are generated, enter early_with_info. To display only the links to passing students as soon as certificates are generated, enter early_no_info.
###### Notice that the value of this property should be in a pair of quotes
```
certificates_display_behavior:"early_with_info"
```
---
#### Course Card Image (Course Image)	
###### It indicates what image will be used as the course image
###### Notice that the value of this property should be in a pair of quotes
```
course_image:"images_course_image.jpg"
```
---
#### Course Display Name	
###### It indicates what name will be used as the name in the course list
###### the $CourseTitle$ is a placeholder of Course Title, code will use the real course title to replace it
###### Notice that the value of this property should be in a pair of quotes
```
display_name:"$CourseTitle$"
```
---
#### Course Number Display String	
###### Enter the course number that you want to appear in the course. 
###### Notice that the value of this property should be in a pair of quotes
```
display_coursenumber:""
```
---
#### Course Visibility In Catalog
###### Defines the access permissions for showing the course in the course catalog. This can be set to one of three values: 'both' (show in catalog and allow access to about page), 'about' (only allow access to about page), 'none' (do not show in catalog and do not allow access to an about page).
###### Notice that the value of this property should be in a pair of quotes
```
catalog_visibility:"none"
```

---
#### LTI Passports	
###### Enter the passports for course LTI tools in the following format: "id:client_key:client_secret".
###### This property only accept the regular json data, please be careful with the usage of comma, colon, quotes
```
lti_passports:[
    "passportid1:key1:secret1",
    "passportid2:key2:secret2"
]
```
---
#### Maximum Attempts
###### Enter the maximum number of times a student can try to answer problems. By default, Maximum Attempts is set to 2, if it is set to null, meaning that students have an unlimited number of attempts for problems. You can override this course-wide setting for individual problems. However, if the course-wide setting is a specific number, you cannot set the Maximum Attempts for individual problems to unlimited.
```
max_attempts:2
```

---

# Grading Setting
#### Overall Grade Range	
###### This property only accept the regular json data, please be careful with the usage of comma, colon, quotes
```
GRADE_CUTOFFS: {
		"Pass":0.75
    }
```
---
#### GRADER
###### This property only accept the regular json data, please be careful with the usage of comma, colon, quotes
```
GRADER: [
        {
            "drop_count": 0, 
            "min_count": 4, 
            "short_label": "Quiz", 
            "type": "Knowledge Check", 
            "weight": 0.4
        }, 
        {
            "drop_count": 0, 
            "min_count": 1, 
            "short_label": "Lab", 
            "type": "Lab", 
            "weight": 0.3
        },
        {
            "drop_count": 0, 
            "min_count": 1, 
            "short_label": "Final", 
            "type": "Final Exam", 
            "weight": 0.3
        }
    ]
```
---
#### LTI Passports	
###### Enter the passports for course LTI tools in the following format: "id:client_key:client_secret".
###### Put the passport name (with quotation marks) in square brackets, and separates each using comma. 
```
lti_passports:[
    "xtreme:LeX:9B059015095B4BF89E6176E992AE6BCC"
] 
```
---

# Schedule And Details Settings

#### Course Pacing	
###### It indicates if enable Self-Paced
###### allowed Value: true or false
###### if assigns to 'false', the platform use Instructor-Paced mode. otherwise (assigns to 'true'), the platform use Self-paced mode.
###### Instructor-paced courses progress at the pace that the course author sets. You can configure release dates for course content and due dates for assignments.
###### Self-paced courses do not have release dates for course content or due dates for assignments. Learners can complete course material at any time before the course end date.

```
self_paced:true
```
---

#### Course Start Date
###### First day the course begins
###### Notice that the value of this property should be in a pair of quotes

```
start: "2017-08-08T01:00:00Z"
```
---

#### Course End Date
###### Last day your course is active
###### Notice that the value of this property should be in a pair of quotes

```
end: "2027-12-31T23:59:00Z"
```
---


#### Enrollment Start Date
###### First day students can enroll
###### Notice that the value of this property should be in a pair of quotes

```
enrollment_start: "2017-08-08T01:00:00Z"
```
---


#### Enrollment End Date
###### Last day students can enroll
###### Notice that the value of this property should be in a pair of quotes

```
enrollment_end: "2027-12-31T23:59:00Z"
```
---


#### Language	
###### Identify the course language here. This is used to assist users find courses that are taught in a specific language.
###### Use the Language Codes to identifu the language.
###### Notice that the value of this property should be in a pair of quotes
```
Language:"en"
```
---


#### Hours of Effort in total	
###### Time spent on all course work.
###### Notice that the value of this property should be in a pair of quotes
```
effort:"14-26 hours in total"
```
---


#### Course Short Description	
###### Appears on the course catalog page when students roll over the course name. Limit to ~150 characters
###### Notice that the value of this property should be in a pair of quotes
```
course_short_description:"This is the course short description1"
```
---

#### Course Introduction Video	
###### Enter your YouTube video's ID (along with any restriction parameters)
###### Notice that the value of this property should be in a pair of quotes
```
about_video_id:"3_yD_cEKoCk"
```
---


# Other Settings
---
#### Video Upload Credentials
###### The unique identifier for your course's video files provided by edX
###### This property only accept the regular json data, please be careful with the usage of comma, colon, quotes

```
video_upload_pipeline:{
 "course_video_upload_token":"958caaa64c6611e7af70127a4fc0bc92"
}
```
---