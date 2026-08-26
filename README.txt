CAV Survey FINAL

This package contains the frozen questionnaire content.

PILOT
-----
Use the PILOT package first for the soft launch.
Its index.html has:
study_phase = pilot
version = 2.0-final

MAIN
----
After reviewing the pilot and deciding that no semantic/questionnaire changes are needed,
deploy the MAIN package.
Its index.html has:
study_phase = main
version = 2.0-final

Both versions have identical questionnaire content. Only the study phase and local storage
namespace differ.

Final content changes:
- Removed the optional open-ended final question.
- On the successful submission page:
  - keeps “退出问卷”
  - fresh same-device response button reads “再次作答”
- The balanced 27-block randomization, 4 profiles/respondent, 5 repeated outcomes,
  15-item deep module, B×C design, quality control and Supabase upload are unchanged.

GitHub final live files should ultimately be:
- index.html
- admin.html

Supabase:
Run FINAL_supabase_once.sql once before the pilot/main deployment.
