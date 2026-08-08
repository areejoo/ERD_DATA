# أمثلة بيانات مخطط قاعدة البيانات

> كل جدول يحتوي على اسم العمود وثلاثة أمثلة للقيم. جميع قيم `id` ممثلة كأرقام صحيحة `INT`.

## task_types
أنواع المهام المستخدمة لتصنيف مهام البطاقات الوظيفية.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| code | PRIMARY | SUPPORT | SUPERVISORY |
| name_ar | مهام رئيسية | مهام مساندة | مهام إشرافية |
| name_en | Primary Tasks | Supporting Tasks | Supervisory Tasks |
| is_active | true | true | true |

---

## job_categories
تصنيفات الوظائف.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| code | — | — | — |
| name_ar | ادارة وسطى | مراقب أشغال | ادارة عليا |
| name_en | — | — | — |
| is_active | true | true | true |

---

## job_definitions
التعريف الأساسي للمسميات الوظيفية.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| code | JOB-001 | JOB-002 | JOB-003 |
| name_ar | مدير الموارد البشرية | أخصائي موارد بشرية | محلل موارد بشرية |
| name_en | HR Director | HR Specialist | HR Analyst |
| is_active | true | true | true |

---

## career_tracks
المسارات المهنية التي تصنف تطور الوظائف.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| code | MGMT | PROF | TECH |
| name_ar | المسار الإداري | المسار التخصصي | المسار التقني |
| name_en | Management | Professional | Technical |
| is_active | true | true | true |

---

## qualifications
المؤهلات العلمية التي يمكن ربطها بالوظائف.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| code | DIPLOMA | BACHELOR | MASTER |
| name_ar | هندسة مدني | ماستر في الادارة | معهد حاسوب |
| name_en | Diploma | Bachelor | Master |
| level | 5 | 6 | 7 |
| is_active | true | true | true |

---

## job_groups
مجموعات تستخدم لتجميع الوظائف حسب طبيعتها أو مستواها.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| code | EXEC | SPEC | ADMIN |
| name_ar | الوظائف القيادية | الوظائف التخصصية | الوظائف الإدارية |
| name_en | Executive Jobs | Specialist Jobs | Administrative Jobs |
| description | وظائف الإدارة العليا | وظائف تتطلب تخصصاً مهنياً | وظائف الدعم الإداري |
| is_active | true | true | true |

---

## org_units
الوحدات التنظيمية الهرمية مثل الإدارات والأقسام.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| code | MUN | HR | RECRUIT |
| name_ar | رئاسة المجلس | مديريةة التنمية الادارية | دائرة شؤون العاملين |
| name_en | — | H | — |
| description | الوحدة التنظيمية الرئيسية | إدارة الموارد البشرية | قسم مسؤول عن بيانات العاميلن... |
| parent_unit_id | NULL | 1 | 2 |
| node_type | رئيس مجلس | مديرية | دائرة |
| is_active | true | true | true |

---

## org_structures
إصدارات الهياكل التنظيمية وحالة اعتماد كل إصدار.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| name_ar | الهيكل التنظيمي 2025 | الهيكل التنظيمي 2026 | تحديث الهيكل 2026 |
| name_en | Org Structure 2025 | Org Structure 2026 | Org Structure Update |
| version | 1.0 | 2.0 | 2.1 |
| status | EXPIRED | APPROVED | IN_REVIEW |
| description | الإصدار السابق | الإصدار الحالي | ممكن يجهزو تحديث مقترح للسنة الجاية |
| effective_date | 2025-01-01 | 2026-01-01 | 2026-09-01 |
| expiry_date | 2025-12-31 | 2026-12-31 | 2027-12-31 |
| current_approval_instance_id | 1 | 2 | 3 |
| approved_at | 2024-12-20 | 2025-12-20 | NULL |
| approved_by | 3 | 3 | NULL |

---

## job_structures
إصدارات هيكل الوظائف.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| name_ar | هيكل الوظائف 2025 | هيكل الوظائف 2026 | تحديث هيكل الوظائف |
| name_en | Job Structure 2025 | Job Structure 2026 | Job Structure Update |
| version | 1.0 | 2.0 | 2.1 |
| status | EXPIRED | APPROVED | IN_REVIEW |
| description | الإصدار السابق | الإصدار الحالي | تحديث مقترح |
| effective_date | 2025-01-01 | 2026-01-01 | 2026-09-01 |
| expiry_date | 2025-12-31 | 2026-12-31 | 2027-12-31 |
| current_approval_instance_id | 1 | 2 | 3 |
| approved_at | 2024-12-22 | 2025-12-22 | NULL |
| approved_by | 3 | 3 | NULL |

---

## job_structure_org_structure
يربط بين إصدارات هيكل الوظائف وإصدارات الهيكل التنظيمي.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| job_structure_id | 1 | 2 | 3 |
| org_structure_id | 1 | 2 | 3 |
| linked_at | 2025-01-01 09:00 | 2026-01-01 09:00 | 2026-09-01 09:00 |
| linked_by | 1 | 1 | 2 |

---

## job_structure_entries
الوظائف الموجودة داخل كل إصدار من هيكل الوظائف وتسلسلها.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| job_structure_id | 2 | 2 | 2 |
| job_definition_id | 1 | 2 | 3 |
| parent_entry_id | NULL | 1 | 1 |
| job_group_id | 1 | 2 | 2 |
| career_track_id | 1 | 2 | 2 |
| max_headcount | 1 | 5 | 3 |
| current_active_vacancies | 0 | 2 | 1 |
| sort_order | 1 | 2 | 3 |

---

## job_entry_qualifications
يربط وظائف الهيكل بالمؤهلات المطلوبة، لأن الوظيفة الواحدة قد تحتاج شهادة أو أكثر.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| job_entry_id | 1 | 2 | 3 |
| qualification_id | 3 | 2 | 2 |
| is_preferred | true | false | true |

---

## job_cards
البطاقة التفصيلية للوظيفة وربطها بالوحدة والتصنيف.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| job_definition_id | 1 | 2 | 3 |
| org_unit_id | 2 | 2 | 3 |
| job_id | 1 | 2 | 3 |
| direct_manager_job_id | NULL | 1 | 1 |
| deputy_job_id | 2 | 3 | NULL |
| category_id | 1 | 2 | 2 |
| status | APPROVED | APPROVED | IN_REVIEW |
| current_approval_instance_id | 1 | 2 | 3 |

---

## job_card_tasks
المهام الفعلية المدرجة داخل كل بطاقة وظيفية.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| job_card_id | 1 | 2 | 3 |
| task_type_id | 3 | 1 | 2 |
| description | الإشراف على استراتيجية الموارد البشرية | إعداد تقارير التوظيف | تحليل مؤشرات الموارد البشرية |
| sort_order | 1 | 1 | 2 |

---

## vacancy_type
أنواع الشواغر، مثل الشاغر من أصل الهيكل الوظيفي أو الشاغر المحدث حكماً.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| code | Base | — | New |
| name_ar | شاغر وظيفي | — | شاغر محدث حكما |
| name_en | Base Position | — | New Vacancy |
| is_active | true | true | true |

---

## vacancies
الشواغر الفردية وحالتها والوظيفة المرتبطة بها.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| job_definition_id | 2 | 3 | NULL |
| vacancy_code | VAC-2026-001 | VAC-2026-002 | VAC-2026-003 |
| status | VACANT | OCCUPIED | FROZEN |
| vacancy_type_id | 1 | 2 | 3 |

---

## templates
قوالب تستخدم في إنشاء طلبات الشواغر والمراسلات، وستوضح لاحقاً.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |

---

## vacancy_requests
طلبات إحداث أو إلغاء الشواغر ومصدر الطلب وحالته، وهو الجدول الأب لتفاصيل الطلب.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| origin_type | MINISTRY_DECREE | INTERNAL_REQUEST | INTERNAL_REQUEST |
| template_id | 1 | 2 | 3 |
| title | طلب إحداث وظائف | طلب إلغاء شاغر | طلب طي شاغر |
| header_content | قرار وزاري رقم 101 | إلى إدارة الموارد البشرية | إلى لجنة الوظائف |
| body_content | إحداث ثلاثة شواغر جديدة | إلغاء الشاغر المجمد | طلب إحلال موظف متقاعد |
| footer_content | مع التحية | وتفضلوا بقبول الاحترام | مع الشكر |
| status | APPROVED | PENDING | REJECTED |
| attachment_id | 1 | 2 | 3 |

---

## vacancy_request_details
تفاصيل الوظائف أو الشواغر المشمولة داخل كل طلب.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| request_id | 1 | 2 | 3 |
| vacancy_id | NULL | 3 | 2 |
| job_definition_id | 2 | NULL | 3 |

---

## attachments
المرفقات المركزية المرتبطة بكيانات النظام بطريقة Polymorphic Association.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| entity_type | vacancy_request | لاحقا رح يصير جدول اسمه تعميم | — |
| entity_id | 1 | 2 | — |
| file_name | قرار_إحداث.pdf | 'طي شاغر'.pdf | — |
| file_path | /docs/decision-101.pdf | /docs/cancel-002.pdf | f |
| file_size_kb | 845 | 420 | 610 |
| mime_type | application/pdf | application/pdf | application/pdf |
| uploaded_at | 2026-03-01 10:30 | 2026-03-05 11:00 | 2026-03-08 09:15 |
| uploaded_by | 2 | 2 | 1 |
| doc_number | 101 | 102 | 103 |
| doc_date | 2026-02-28 | 2026-03-04 | 2026-03-07 |

---

## workflow_rules
قواعد وخطوات مسار الموافقة حسب نوع الكيان والدور المطلوب.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| entity_type | vacancy_request | لاحقا رح يصير جدول اسمه تعميم | اجازة مثلا جدول بكون |
| step_order | 1 | 2 | 1 |
| role_code | HR_OFFICER | HR_MANAGER | CITY_MANAGER |
| step_name | مراجعة الطلب | اعتماد الموارد البشرية | اعتماد التعميم |

---

## approval_instances
نسخة تنفيذية لمسار موافقة خاص بكيان أو جدول محدد يتطلب موافقات.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| entity_type | vacancy_request | vacancy_request | ORG_STRUCTURE |
| entity_id | 1 | 2 | 2 |
| status | Approved | Approved | REJECTED |
| current_step | 3 | 2 | 2 |
| started_at | 2026-03-01 09:00 | 2026-03-05 09:30 | 2026-03-07 08:45 |
| completed_at | 2026-03-03 14:00 | NULL | 2026-03-08 12:00 |

---

## approval_instance_steps
تفاصيل كل خطوة ضمن نسخة الموافقة وحالتها ومن نفذها.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| approval_instance_id | 1 | 1 | 2 |
| step_order | 1 | 2 | 1 |
| role_code | HR_OFFICER | HR_MANAGER | HR_OFFICER |
| status | APPROVED | APPROVED | PENDING |
| action_by | 4 | 5 | NULL |
| action_at | 2026-03-01 12:00 | 2026-03-02 15:30 | NULL |

---

## users
المستخدمون المسجلون في النظام.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |

---

## roles
الأدوار التي يمكن إسنادها للمستخدمين.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| role_code | CITY_MANAGER | HR_MANAGER | HR_OFFICER |
| role_name | مدير الأمانة | مدير الموارد البشرية | مسؤول الموارد البشرية |

---

## permissions
الصلاحيات والعمليات التي يمكن منحها للأدوار.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| id | 1 | 2 | 3 |
| permission_code | CAN_APPROVE_VACANCY | CAN_MANAGE_JOB_STRUCTURE | CAN_REVIEW_REQUEST |
| description | اعتماد طلبات الشواغر | إدارة هيكل الوظائف | مراجعة الطلبات |

---

## role_permissions
جدول وسيط يربط الأدوار بالصلاحيات.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| role_id | 1 | 2 | 3 |
| permission_id | 1 | 2 | 3 |

---

## user_roles
جدول وسيط يربط المستخدمين بالأدوار.

| اسم العمود | مثال 1 | مثال 2 | مثال 3 |
|---|---|---|---|
| user_id | 1 | 2 | 3 |
| role_id | 1 | 2 | 3 |
