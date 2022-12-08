







<!DOCTYPE html>
<html lang="en" data-color-mode="auto" data-light-theme="light" data-dark-theme="dark" data-a11y-animated-images="system">
  <head>
    <meta charset="utf-8">
  <script type="text/javascript" nonce="4faf493616e149d7b31add6e782" src="//local.adguard.org?ts=1670476889175&amp;type=content-script&amp;dmn=github.com&amp;pth=%2Fsean207cc%2FAI-course%2Fblob%2Fgh-pages%2F_posts%2F2022-12-08-Pose-Estimation.md&amp;app=com.apple.Safari&amp;css=2&amp;js=1&amp;rel=1&amp;rji=1&amp;sbe=1&amp;stealth=1&amp;st-push&amp;st-loc&amp;st-java&amp;st-dnt"></script>
<script type="text/javascript" nonce="4faf493616e149d7b31add6e782" src="//local.adguard.org?ts=1670476889175&amp;name=Web%20of%20Trust&amp;name=AdGuard%20Popup%20Blocker&amp;name=AdGuard%20Extra&amp;type=user-script"></script><link rel="dns-prefetch" href="https://github.githubassets.com">
  <link rel="dns-prefetch" href="https://avatars.githubusercontent.com">
  <link rel="dns-prefetch" href="https://github-cloud.s3.amazonaws.com">
  <link rel="dns-prefetch" href="https://user-images.githubusercontent.com/">
  <link rel="preconnect" href="https://github.githubassets.com" crossorigin>
  <link rel="preconnect" href="https://avatars.githubusercontent.com">



  <link crossorigin="anonymous" media="all" rel="stylesheet" href="https://github.githubassets.com/assets/light-719f1193e0c0.css" /><link crossorigin="anonymous" media="all" rel="stylesheet" href="https://github.githubassets.com/assets/dark-0c343b529849.css" /><link data-color-theme="dark_dimmed" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/dark_dimmed-f22da508b62a.css" /><link data-color-theme="dark_high_contrast" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/dark_high_contrast-188ef1de59e6.css" /><link data-color-theme="dark_colorblind" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/dark_colorblind-bc6bf4eea850.css" /><link data-color-theme="light_colorblind" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/light_colorblind-527658dec362.css" /><link data-color-theme="light_high_contrast" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/light_high_contrast-c7a7fe0cd8ec.css" /><link data-color-theme="light_tritanopia" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/light_tritanopia-6aa855bdae0f.css" /><link data-color-theme="dark_tritanopia" crossorigin="anonymous" media="all" rel="stylesheet" data-href="https://github.githubassets.com/assets/dark_tritanopia-6aa5e25aacc0.css" />
  
    <link crossorigin="anonymous" media="all" rel="stylesheet" href="https://github.githubassets.com/assets/primer-cd5f115a3ed9.css" />
    <link crossorigin="anonymous" media="all" rel="stylesheet" href="https://github.githubassets.com/assets/global-4bc9b3a08d31.css" />
    <link crossorigin="anonymous" media="all" rel="stylesheet" href="https://github.githubassets.com/assets/github-ed372cf0a5db.css" />
  <link crossorigin="anonymous" media="all" rel="stylesheet" href="https://github.githubassets.com/assets/code-7821b0df4109.css" />

    <meta name="optimizely-datafile" content="{&quot;groups&quot;: [], &quot;environmentKey&quot;: &quot;production&quot;, &quot;rollouts&quot;: [], &quot;typedAudiences&quot;: [], &quot;projectId&quot;: &quot;16737760170&quot;, &quot;variables&quot;: [], &quot;featureFlags&quot;: [], &quot;experiments&quot;: [], &quot;version&quot;: &quot;4&quot;, &quot;audiences&quot;: [{&quot;conditions&quot;: &quot;[\&quot;or\&quot;, {\&quot;match\&quot;: \&quot;exact\&quot;, \&quot;name\&quot;: \&quot;$opt_dummy_attribute\&quot;, \&quot;type\&quot;: \&quot;custom_attribute\&quot;, \&quot;value\&quot;: \&quot;$opt_dummy_value\&quot;}]&quot;, &quot;id&quot;: &quot;$opt_dummy_audience&quot;, &quot;name&quot;: &quot;Optimizely-Generated Audience for Backwards Compatibility&quot;}], &quot;anonymizeIP&quot;: true, &quot;sdkKey&quot;: &quot;WTc6awnGuYDdG98CYRban&quot;, &quot;attributes&quot;: [{&quot;id&quot;: &quot;16822470375&quot;, &quot;key&quot;: &quot;user_id&quot;}, {&quot;id&quot;: &quot;17143601254&quot;, &quot;key&quot;: &quot;spammy&quot;}, {&quot;id&quot;: &quot;18175660309&quot;, &quot;key&quot;: &quot;organization_plan&quot;}, {&quot;id&quot;: &quot;18813001570&quot;, &quot;key&quot;: &quot;is_logged_in&quot;}, {&quot;id&quot;: &quot;19073851829&quot;, &quot;key&quot;: &quot;geo&quot;}, {&quot;id&quot;: &quot;20175462351&quot;, &quot;key&quot;: &quot;requestedCurrency&quot;}, {&quot;id&quot;: &quot;20785470195&quot;, &quot;key&quot;: &quot;country_code&quot;}, {&quot;id&quot;: &quot;21656311196&quot;, &quot;key&quot;: &quot;opened_downgrade_dialog&quot;}], &quot;botFiltering&quot;: false, &quot;accountId&quot;: &quot;16737760170&quot;, &quot;events&quot;: [{&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;17911811441&quot;, &quot;key&quot;: &quot;hydro_click.dashboard.teacher_toolbox_cta&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18124116703&quot;, &quot;key&quot;: &quot;submit.organizations.complete_sign_up&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18145892387&quot;, &quot;key&quot;: &quot;no_metric.tracked_outside_of_optimizely&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18178755568&quot;, &quot;key&quot;: &quot;click.org_onboarding_checklist.add_repo&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18180553241&quot;, &quot;key&quot;: &quot;submit.repository_imports.create&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18186103728&quot;, &quot;key&quot;: &quot;click.help.learn_more_about_repository_creation&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18188530140&quot;, &quot;key&quot;: &quot;test_event&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18191963644&quot;, &quot;key&quot;: &quot;click.empty_org_repo_cta.transfer_repository&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18195612788&quot;, &quot;key&quot;: &quot;click.empty_org_repo_cta.import_repository&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18210945499&quot;, &quot;key&quot;: &quot;click.org_onboarding_checklist.invite_members&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18211063248&quot;, &quot;key&quot;: &quot;click.empty_org_repo_cta.create_repository&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18215721889&quot;, &quot;key&quot;: &quot;click.org_onboarding_checklist.update_profile&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18224360785&quot;, &quot;key&quot;: &quot;click.org_onboarding_checklist.dismiss&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18234832286&quot;, &quot;key&quot;: &quot;submit.organization_activation.complete&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18252392383&quot;, &quot;key&quot;: &quot;submit.org_repository.create&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18257551537&quot;, &quot;key&quot;: &quot;submit.org_member_invitation.create&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18259522260&quot;, &quot;key&quot;: &quot;submit.organization_profile.update&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18564603625&quot;, &quot;key&quot;: &quot;view.classroom_select_organization&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18568612016&quot;, &quot;key&quot;: &quot;click.classroom_sign_in_click&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18572592540&quot;, &quot;key&quot;: &quot;view.classroom_name&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18574203855&quot;, &quot;key&quot;: &quot;click.classroom_create_organization&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18582053415&quot;, &quot;key&quot;: &quot;click.classroom_select_organization&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18589463420&quot;, &quot;key&quot;: &quot;click.classroom_create_classroom&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18591323364&quot;, &quot;key&quot;: &quot;click.classroom_create_first_classroom&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18591652321&quot;, &quot;key&quot;: &quot;click.classroom_grant_access&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18607131425&quot;, &quot;key&quot;: &quot;view.classroom_creation&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;18831680583&quot;, &quot;key&quot;: &quot;upgrade_account_plan&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;19064064515&quot;, &quot;key&quot;: &quot;click.signup&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;19075373687&quot;, &quot;key&quot;: &quot;click.view_account_billing_page&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;19077355841&quot;, &quot;key&quot;: &quot;click.dismiss_signup_prompt&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;19079713938&quot;, &quot;key&quot;: &quot;click.contact_sales&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;19120963070&quot;, &quot;key&quot;: &quot;click.compare_account_plans&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;19151690317&quot;, &quot;key&quot;: &quot;click.upgrade_account_cta&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;19424193129&quot;, &quot;key&quot;: &quot;click.open_account_switcher&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;19520330825&quot;, &quot;key&quot;: &quot;click.visit_account_profile&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;19540970635&quot;, &quot;key&quot;: &quot;click.switch_account_context&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;19730198868&quot;, &quot;key&quot;: &quot;submit.homepage_signup&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;19820830627&quot;, &quot;key&quot;: &quot;click.homepage_signup&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;19988571001&quot;, &quot;key&quot;: &quot;click.create_enterprise_trial&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20036538294&quot;, &quot;key&quot;: &quot;click.create_organization_team&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20040653299&quot;, &quot;key&quot;: &quot;click.input_enterprise_trial_form&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20062030003&quot;, &quot;key&quot;: &quot;click.continue_with_team&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20068947153&quot;, &quot;key&quot;: &quot;click.create_organization_free&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20086636658&quot;, &quot;key&quot;: &quot;click.signup_continue.username&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20091648988&quot;, &quot;key&quot;: &quot;click.signup_continue.create_account&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20103637615&quot;, &quot;key&quot;: &quot;click.signup_continue.email&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20111574253&quot;, &quot;key&quot;: &quot;click.signup_continue.password&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20120044111&quot;, &quot;key&quot;: &quot;view.pricing_page&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20152062109&quot;, &quot;key&quot;: &quot;submit.create_account&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20165800992&quot;, &quot;key&quot;: &quot;submit.upgrade_payment_form&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20171520319&quot;, &quot;key&quot;: &quot;submit.create_organization&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20222645674&quot;, &quot;key&quot;: &quot;click.recommended_plan_in_signup.discuss_your_needs&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20227443657&quot;, &quot;key&quot;: &quot;submit.verify_primary_user_email&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20234607160&quot;, &quot;key&quot;: &quot;click.recommended_plan_in_signup.try_enterprise&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20238175784&quot;, &quot;key&quot;: &quot;click.recommended_plan_in_signup.team&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20239847212&quot;, &quot;key&quot;: &quot;click.recommended_plan_in_signup.continue_free&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20251097193&quot;, &quot;key&quot;: &quot;recommended_plan&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20438619534&quot;, &quot;key&quot;: &quot;click.pricing_calculator.1_member&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20456699683&quot;, &quot;key&quot;: &quot;click.pricing_calculator.15_members&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20467868331&quot;, &quot;key&quot;: &quot;click.pricing_calculator.10_members&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20476267432&quot;, &quot;key&quot;: &quot;click.trial_days_remaining&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20476357660&quot;, &quot;key&quot;: &quot;click.discover_feature&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20479287901&quot;, &quot;key&quot;: &quot;click.pricing_calculator.custom_members&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20481107083&quot;, &quot;key&quot;: &quot;click.recommended_plan_in_signup.apply_teacher_benefits&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20483089392&quot;, &quot;key&quot;: &quot;click.pricing_calculator.5_members&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20484283944&quot;, &quot;key&quot;: &quot;click.onboarding_task&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20484996281&quot;, &quot;key&quot;: &quot;click.recommended_plan_in_signup.apply_student_benefits&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20486713726&quot;, &quot;key&quot;: &quot;click.onboarding_task_breadcrumb&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20490791319&quot;, &quot;key&quot;: &quot;click.upgrade_to_enterprise&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20491786766&quot;, &quot;key&quot;: &quot;click.talk_to_us&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20494144087&quot;, &quot;key&quot;: &quot;click.dismiss_enterprise_trial&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20499722759&quot;, &quot;key&quot;: &quot;completed_all_tasks&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20500710104&quot;, &quot;key&quot;: &quot;completed_onboarding_tasks&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20513160672&quot;, &quot;key&quot;: &quot;click.read_doc&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20516196762&quot;, &quot;key&quot;: &quot;actions_enabled&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20518980986&quot;, &quot;key&quot;: &quot;click.dismiss_trial_banner&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20535446721&quot;, &quot;key&quot;: &quot;click.issue_actions_prompt.dismiss_prompt&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20557002247&quot;, &quot;key&quot;: &quot;click.issue_actions_prompt.setup_workflow&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20595070227&quot;, &quot;key&quot;: &quot;click.pull_request_setup_workflow&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20626600314&quot;, &quot;key&quot;: &quot;click.seats_input&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20642310305&quot;, &quot;key&quot;: &quot;click.decrease_seats_number&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20662990045&quot;, &quot;key&quot;: &quot;click.increase_seats_number&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20679620969&quot;, &quot;key&quot;: &quot;click.public_product_roadmap&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20761240940&quot;, &quot;key&quot;: &quot;click.dismiss_survey_banner&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20767210721&quot;, &quot;key&quot;: &quot;click.take_survey&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20795281201&quot;, &quot;key&quot;: &quot;click.archive_list&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20966790249&quot;, &quot;key&quot;: &quot;contact_sales.submit&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20996500333&quot;, &quot;key&quot;: &quot;contact_sales.existing_customer&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;20996890162&quot;, &quot;key&quot;: &quot;contact_sales.blank_message_field&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21000470317&quot;, &quot;key&quot;: &quot;contact_sales.personal_email&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21002790172&quot;, &quot;key&quot;: &quot;contact_sales.blank_phone_field&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21354412592&quot;, &quot;key&quot;: &quot;click.dismiss_create_readme&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21366102546&quot;, &quot;key&quot;: &quot;click.dismiss_zero_user_content&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21370252505&quot;, &quot;key&quot;: &quot;account_did_downgrade&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21370840408&quot;, &quot;key&quot;: &quot;click.cta_create_readme&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21375451068&quot;, &quot;key&quot;: &quot;click.cta_create_new_repository&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21385390948&quot;, &quot;key&quot;: &quot;click.zero_user_content&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21467712175&quot;, &quot;key&quot;: &quot;click.downgrade_keep&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21484112202&quot;, &quot;key&quot;: &quot;click.downgrade&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21495292213&quot;, &quot;key&quot;: &quot;click.downgrade_survey_exit&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21508241468&quot;, &quot;key&quot;: &quot;click.downgrade_survey_submit&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21512030356&quot;, &quot;key&quot;: &quot;click.downgrade_support&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21539090022&quot;, &quot;key&quot;: &quot;click.downgrade_exit&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21543640644&quot;, &quot;key&quot;: &quot;click_fetch_upstream&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21646510300&quot;, &quot;key&quot;: &quot;click.move_your_work&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21656151116&quot;, &quot;key&quot;: &quot;click.add_branch_protection_rule&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21663860599&quot;, &quot;key&quot;: &quot;click.downgrade_dialog_open&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21687860483&quot;, &quot;key&quot;: &quot;click.learn_about_protected_branches&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21689050333&quot;, &quot;key&quot;: &quot;click.dismiss_protect_this_branch&quot;}, {&quot;experimentIds&quot;: [], &quot;id&quot;: &quot;21864370109&quot;, &quot;key&quot;: &quot;click.sign_in&quot;}], &quot;revision&quot;: &quot;1367&quot;}" />


  <script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/wp-runtime-53402cbac3d8.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_smoothscroll-polyfill_dist_smoothscroll_js-node_modules_stacktrace-parse-297da6-aaa32681a0b3.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/environment-ebb879fbdb40.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_selector-observer_dist_index_esm_js-650337916dbd.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_delegated-events_dist_index_js-node_modules_github_details-dialog-elemen-63debe-4a2f37f7419e.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_fzy_js_index_js-node_modules_github_markdown-toolbar-element_dist_index_js-5936f45973f5.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_github_filter-input-element_dist_index_js-node_modules_github_remote-inp-73b750-ab4920e0b37a.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_github_file-attachment-element_dist_index_js-node_modules_github_text-ex-3415a8-daf4603c6e6b.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_primer_view-components_app_components_primer_primer_js-node_modules_gith-aa5398-aca9d5983f34.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/github-elements-8bcd745975ba.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/element-registry-a67d4661e8bb.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_lit-html_lit-html_js-e954e8c01c93.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_github_catalyst_lib_index_js-node_modules_github_hydro-analytics-client_-17abfd-e5695ecb0f0c.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_manuelpuyol_turbo_dist_turbo_es2017-esm_js-af11d99b3e65.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_github_alive-client_dist_index_js-156187f13fbb.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_github_mini-throttle_dist_index_js-node_modules_github_remote-form_dist_-ece2b0-917c0dad4566.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_primer_behaviors_dist_esm_dimensions_js-node_modules_github_jtml_lib_index_js-c1acb9a3f5fa.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_github_paste-markdown_dist_index_esm_js-node_modules_github_quote-select-f12f19-f987ad18f3a3.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/app_assets_modules_github_aria-live_ts-app_assets_modules_github_hydro-analytics_ts-app_asset-7c220e-f3c6c718b3ec.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/app_assets_modules_github_updatable-content_ts-62df1309213c.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/app_assets_modules_github_sticky-scroll-into-view_ts-39278b4d6f66.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/app_assets_modules_github_behaviors_keyboard-shortcuts-helper_ts-app_assets_modules_github_be-f5afdb-e0346850e585.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/app_assets_modules_github_behaviors_commenting_edit_ts-app_assets_modules_github_behaviors_ht-83c235-cb56bba555dc.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/behaviors-68f99cb643cf.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_delegated-events_dist_index_js-node_modules_github_catalyst_lib_index_js-06ff532-0eddb8f4d122.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/notifications-global-35a509648d46.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_optimizely_optimizely-sdk_dist_optimizely_browser_es_min_js-node_modules-77839b-550a5f909f1b.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/optimizely-0db0f6a6e783.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/react-lib-a3151b3a4edd.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_primer_react_lib-esm_BaseStyles_js-node_modules_primer_react_lib-esm_Box-6e6e3d-078007b31175.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_virtualized-list_es_index_js-node_modules_github_template-parts_lib_index_js-8b135c9d75cf.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_github_filter-input-element_dist_index_js-node_modules_github_mini-throt-31d1eb-ead65925a38e.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_github_file-attachment-element_dist_index_js-node_modules_github_mini-th-85225b-d5c5eb0b8bb2.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/app_assets_modules_react-core_register-react-app_ts-9328c01359aa.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/app_assets_modules_github_ref-selector_ts-2ef6ded89582.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/repositories-3332672f4f00.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_github_clipboard-copy-element_dist_index_esm_js-node_modules_github_remo-f81170-4387707a2af3.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_github_mini-throttle_dist_decorators_js-node_modules_scroll-anchoring_di-e71893-bd36a94892da.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/app_assets_modules_github_diffs_blob-lines_ts-app_assets_modules_github_diffs_linkable-line-n-dca161-72425918bcd8.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/diffs-a36cd214f3c5.js"></script>
  

  <title>AI-course/2022-12-08-Pose-Estimation.md at gh-pages · sean207cc/AI-course</title>



    

  <meta name="request-id" content="C95D:0ADC:41728B:4BE440:6391CC9D" data-turbo-transient="true" /><meta name="html-safe-nonce" content="427c9ac94c379f7dc1c287266e374edfdc5fe69a3f480b316921f3b5676cbca4" data-turbo-transient="true" /><meta name="visitor-payload" content="eyJyZWZlcnJlciI6bnVsbCwicmVxdWVzdF9pZCI6IkM5NUQ6MEFEQzo0MTcyOEI6NEJFNDQwOjYzOTFDQzlEIiwidmlzaXRvcl9pZCI6IjI0NjQ0Njk0MDczODQwNzc0NjEiLCJyZWdpb25fZWRnZSI6ImF1c3RyYWxpYWVhc3QiLCJyZWdpb25fcmVuZGVyIjoiaWFkIn0=" data-turbo-transient="true" /><meta name="visitor-hmac" content="0f197e348f3332f3aaf0172ee8d1139f6a299273f3bcca252aaa7dc0950472b1" data-turbo-transient="true" />


    <meta name="hovercard-subject-tag" content="repository:575813281" data-turbo-transient>


  <meta name="github-keyboard-shortcuts" content="repository,source-code,file-tree" data-turbo-transient="true" />
  

  <meta name="selected-link" value="repo_source" data-turbo-transient>

    <meta name="google-site-verification" content="c1kuD-K2HIVF635lypcsWPoD4kilo5-jA_wBFyT4uMY">
  <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
  <meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
  <meta name="google-site-verification" content="GXs5KoUUkNCoaAZn7wPN-t01Pywp9M3sEjnt_3_ZWPc">
  <meta name="google-site-verification" content="Apib7-x98H0j5cPqHWwSMm6dNU4GmODRoqxLiDzdx9I">

<meta name="octolytics-url" content="https://collector.github.com/github/collect" /><meta name="octolytics-actor-id" content="114159512" /><meta name="octolytics-actor-login" content="sean207cc" /><meta name="octolytics-actor-hash" content="698fe9977cf0a9a2c30530ff60bdb0e5d42c311d4e753eb891015ad83ca69810" />

  <meta name="analytics-location" content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-turbo-transient="true" />

  




  

    <meta name="user-login" content="sean207cc">

  <link rel="sudo-modal" href="/sessions/sudo_modal">

    <meta name="viewport" content="width=device-width">
    
      <meta name="description" content="A concise two-column blog theme for Jekyll. Contribute to sean207cc/AI-course development by creating an account on GitHub.">
      <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <meta property="fb:app_id" content="1401488693436528">
    <meta name="apple-itunes-app" content="app-id=1477376905" />
      <meta name="twitter:image:src" content="https://opengraph.githubassets.com/a128556282cf576203a3ce8e4eb057a9663a21dc3ab118495a9f5c92fe1745ff/sean207cc/AI-course" /><meta name="twitter:site" content="@github" /><meta name="twitter:card" content="summary_large_image" /><meta name="twitter:title" content="AI-course/2022-12-08-Pose-Estimation.md at gh-pages · sean207cc/AI-course" /><meta name="twitter:description" content="A concise two-column blog theme for Jekyll. Contribute to sean207cc/AI-course development by creating an account on GitHub." />
      <meta property="og:image" content="https://opengraph.githubassets.com/a128556282cf576203a3ce8e4eb057a9663a21dc3ab118495a9f5c92fe1745ff/sean207cc/AI-course" /><meta property="og:image:alt" content="A concise two-column blog theme for Jekyll. Contribute to sean207cc/AI-course development by creating an account on GitHub." /><meta property="og:image:width" content="1200" /><meta property="og:image:height" content="600" /><meta property="og:site_name" content="GitHub" /><meta property="og:type" content="object" /><meta property="og:title" content="AI-course/2022-12-08-Pose-Estimation.md at gh-pages · sean207cc/AI-course" /><meta property="og:url" content="https://github.com/sean207cc/AI-course" /><meta property="og:description" content="A concise two-column blog theme for Jekyll. Contribute to sean207cc/AI-course development by creating an account on GitHub." />
      
    <link rel="assets" href="https://github.githubassets.com/">
      <link rel="shared-web-socket" href="wss://alive.github.com/_sockets/u/114159512/ws?session=eyJ2IjoiVjMiLCJ1IjoxMTQxNTk1MTIsInMiOjEwMDkxMTg1MDEsImMiOjIyNDgxMDM1MjcsInQiOjE2NzA0OTk1MzN9--975570ddcf1cc31693753fdc5832485114706b69610837b1f417ac84f4737df2" data-refresh-url="/_alive" data-session-id="ef6831b03d9e7cf0cbf84a009a6e506a66144184a7ad54763368f6178fae012f">
      <link rel="shared-web-socket-src" href="/assets-cdn/worker/socket-worker-b87581f5816c.js">


        <meta name="hostname" content="github.com">


      <meta name="keyboard-shortcuts-preference" content="all">
      <script type="application/json" id="memex_keyboard_shortcuts_preference">"all"</script>

        <meta name="expected-hostname" content="github.com">

    <meta name="enabled-features" content="TURBO_EXPERIMENT_RISKY,IMAGE_METRIC_TRACKING,GEOJSON_AZURE_MAPS">


  <meta http-equiv="x-pjax-version" content="f6ad2da3ee74bcfe68e0f69f3d22d1dfc59b7ef2d3360a171be5a74ca4799354" data-turbo-track="reload">
  <meta http-equiv="x-pjax-csp-version" content="40aca5a152a13213a876f7628c466cd600db12fb858cdddccc3f1cc387eb7dad" data-turbo-track="reload">
  <meta http-equiv="x-pjax-css-version" content="ab8b794130f538ddaf9e4375a8709b7b390f31e596546606fe900977b3813c6d" data-turbo-track="reload">
  <meta http-equiv="x-pjax-js-version" content="ff8fe8b53a0798b942cf6372676eccbd43368d0d277068eef422e0040ee8354b" data-turbo-track="reload">

  <meta name="turbo-cache-control" content="no-preview" data-turbo-transient="">

        <meta data-hydrostats="publish">

  <meta name="go-import" content="github.com/sean207cc/AI-course git https://github.com/sean207cc/AI-course.git">

  <meta name="octolytics-dimension-user_id" content="114159512" /><meta name="octolytics-dimension-user_login" content="sean207cc" /><meta name="octolytics-dimension-repository_id" content="575813281" /><meta name="octolytics-dimension-repository_nwo" content="sean207cc/AI-course" /><meta name="octolytics-dimension-repository_public" content="true" /><meta name="octolytics-dimension-repository_is_fork" content="true" /><meta name="octolytics-dimension-repository_parent_id" content="428092919" /><meta name="octolytics-dimension-repository_parent_nwo" content="rkuo2000/AI-course" /><meta name="octolytics-dimension-repository_network_root_id" content="361735956" /><meta name="octolytics-dimension-repository_network_root_nwo" content="zivong/jekyll-theme-hydure" />



    <link rel="canonical" href="https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md" data-turbo-transient>
  <meta name="turbo-body-classes" content="logged-in env-production page-responsive page-blob">


  <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">

  <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">

  <meta name="browser-optimizely-client-errors-url" content="https://api.github.com/_private/browser/optimizely_client/errors">

  <link rel="mask-icon" href="https://github.githubassets.com/pinned-octocat.svg" color="#000000">
  <link rel="alternate icon" class="js-site-favicon" type="image/png" href="https://github.githubassets.com/favicons/favicon.png">
  <link rel="icon" class="js-site-favicon" type="image/svg+xml" href="https://github.githubassets.com/favicons/favicon.svg">

<meta name="theme-color" content="#1e2327">
<meta name="color-scheme" content="light dark" />

  <link rel="apple-touch-icon" href="https://github.githubassets.com/apple-touch-icon.png">
  <link rel="apple-touch-icon" sizes="180x180" href="https://github.githubassets.com/apple-touch-icon-180x180.png">
  <meta name="apple-mobile-web-app-title" content="GitHub">

  <link rel="manifest" href="/manifest.json" crossOrigin="use-credentials">

  </head>

  <body class="logged-in env-production page-responsive page-blob" style="word-wrap: break-word;">
      <div data-turbo-body class="logged-in env-production page-responsive page-blob" style="word-wrap: break-word;">
        


    <div class="position-relative js-header-wrapper ">
      <a href="#start-of-content" class="p-3 color-bg-accent-emphasis color-fg-on-emphasis show-on-focus js-skip-to-content">Skip to content</a>
      <span data-view-component="true" class="progress-pjax-loader Progress position-fixed width-full">
    <span style="width: 0%;" data-view-component="true" class="Progress-item progress-pjax-loader-bar left-0 top-0 color-bg-accent-emphasis"></span>
</span>      
      


        <script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_github_mini-throttle_dist_decorators_js-node_modules_github_command-pale-4090c9-7f4a07119d05.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/vendors-node_modules_github_clipboard-copy-element_dist_index_esm_js-node_modules_delegated-e-b37f7d-a9860783b46f.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/app_assets_modules_github_command-palette_items_help-item_ts-app_assets_modules_github_comman-48ad9d-40964356e9cb.js"></script>
<script crossorigin="anonymous" defer="defer" type="application/javascript" src="https://github.githubassets.com/assets/command-palette-38af56440410.js"></script>

            <header class="Header js-details-container Details px-3 px-md-4 px-lg-5 flex-wrap flex-md-nowrap" role="banner">

    <div class="Header-item mt-n1 mb-n1  d-none d-md-flex">
      <a
  class="Header-link"
  href="https://github.com/"
  data-hotkey="g d"
  aria-label="Homepage "
  data-turbo="false"
  data-analytics-event="{&quot;category&quot;:&quot;Header&quot;,&quot;action&quot;:&quot;go to dashboard&quot;,&quot;label&quot;:&quot;icon:logo&quot;}"
>
  <svg height="32" aria-hidden="true" viewBox="0 0 16 16" version="1.1" width="32" data-view-component="true" class="octicon octicon-mark-github v-align-middle">
    <path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path>
</svg>
</a>

    </div>

    <div class="Header-item d-md-none">
        <button aria-label="Toggle navigation" aria-expanded="false" type="button" data-view-component="true" class="Header-link js-details-target btn-link">    <svg aria-hidden="true" height="24" viewBox="0 0 16 16" version="1.1" width="24" data-view-component="true" class="octicon octicon-three-bars">
    <path fill-rule="evenodd" d="M1 2.75A.75.75 0 011.75 2h12.5a.75.75 0 110 1.5H1.75A.75.75 0 011 2.75zm0 5A.75.75 0 011.75 7h12.5a.75.75 0 110 1.5H1.75A.75.75 0 011 7.75zM1.75 12a.75.75 0 100 1.5h12.5a.75.75 0 100-1.5H1.75z"></path>
</svg>
</button>    </div>

    <div class="Header-item Header-item--full flex-column flex-md-row width-full flex-order-2 flex-md-order-none mr-0 mt-3 mt-md-0 Details-content--hidden-not-important d-md-flex">
              



<div class="header-search flex-auto position-relative js-site-search flex-self-stretch flex-md-self-auto mb-3 mb-md-0 mr-0 mr-md-3 scoped-search site-scoped-search js-jump-to"
>
  <div class="position-relative">
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="js-site-search-form" role="search" aria-label="Site" data-scope-type="Repository" data-scope-id="575813281" data-scoped-search-url="/sean207cc/AI-course/search" data-owner-scoped-search-url="/users/sean207cc/search" data-unscoped-search-url="/search" data-turbo="false" action="/sean207cc/AI-course/search" accept-charset="UTF-8" method="get">
      <label class="form-control header-search-wrapper input-sm p-0 js-chromeless-input-container header-search-wrapper-jump-to position-relative d-flex flex-justify-between flex-items-center">
        <input type="text"
          class="form-control js-site-search-focus header-search-input jump-to-field js-jump-to-field js-site-search-field is-clearable"
          data-hotkey=s,/
          name="q"
          data-test-selector="nav-search-input"
          placeholder="Search or jump to…"
          data-unscoped-placeholder="Search or jump to…"
          data-scoped-placeholder="Search or jump to…"
          autocapitalize="off"
          role="combobox"
          aria-haspopup="listbox"
          aria-expanded="false"
          aria-autocomplete="list"
          aria-controls="jump-to-results"
          aria-label="Search or jump to…"
          data-jump-to-suggestions-path="/_graphql/GetSuggestedNavigationDestinations"
          spellcheck="false"
          autocomplete="off"
        >
        <input type="hidden" value="00FvbIym5-e2UPOmAYLB2mpqiTEZH_zH1ddtGz4waOSRimKzUOgtGkK1j-uDHwpzEJz7fxX31fRLIJNstvYn8A" data-csrf="true" class="js-data-jump-to-suggestions-path-csrf" />
        <input type="hidden" class="js-site-search-type-field" name="type" >
            <svg xmlns="http://www.w3.org/2000/svg" width="22" height="20" aria-hidden="true" class="mr-1 header-search-key-slash"><path fill="none" stroke="#979A9C" opacity=".4" d="M3.5.5h12c1.7 0 3 1.3 3 3v13c0 1.7-1.3 3-3 3h-12c-1.7 0-3-1.3-3-3v-13c0-1.7 1.3-3 3-3z"></path><path fill="#979A9C" d="M11.8 6L8 15.1h-.9L10.8 6h1z"></path></svg>


          <div class="Box position-absolute overflow-hidden d-none jump-to-suggestions js-jump-to-suggestions-container">
            
<ul class="d-none js-jump-to-suggestions-template-container">
  

<li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item js-jump-to-suggestion" role="option">
  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open p-2" href="" data-item-type="suggestion">
    <div class="jump-to-octicon js-jump-to-octicon flex-shrink-0 mr-2 text-center d-none">
      <svg title="Repository" aria-label="Repository" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-repo js-jump-to-octicon-repo d-none flex-shrink-0">
    <path fill-rule="evenodd" d="M2 2.5A2.5 2.5 0 014.5 0h8.75a.75.75 0 01.75.75v12.5a.75.75 0 01-.75.75h-2.5a.75.75 0 110-1.5h1.75v-2h-8a1 1 0 00-.714 1.7.75.75 0 01-1.072 1.05A2.495 2.495 0 012 11.5v-9zm10.5-1V9h-8c-.356 0-.694.074-1 .208V2.5a1 1 0 011-1h8zM5 12.25v3.25a.25.25 0 00.4.2l1.45-1.087a.25.25 0 01.3 0L8.6 15.7a.25.25 0 00.4-.2v-3.25a.25.25 0 00-.25-.25h-3.5a.25.25 0 00-.25.25z"></path>
</svg>
      <svg title="Project" aria-label="Project" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-project js-jump-to-octicon-project d-none flex-shrink-0">
    <path fill-rule="evenodd" d="M1.75 0A1.75 1.75 0 000 1.75v12.5C0 15.216.784 16 1.75 16h12.5A1.75 1.75 0 0016 14.25V1.75A1.75 1.75 0 0014.25 0H1.75zM1.5 1.75a.25.25 0 01.25-.25h12.5a.25.25 0 01.25.25v12.5a.25.25 0 01-.25.25H1.75a.25.25 0 01-.25-.25V1.75zM11.75 3a.75.75 0 00-.75.75v7.5a.75.75 0 001.5 0v-7.5a.75.75 0 00-.75-.75zm-8.25.75a.75.75 0 011.5 0v5.5a.75.75 0 01-1.5 0v-5.5zM8 3a.75.75 0 00-.75.75v3.5a.75.75 0 001.5 0v-3.5A.75.75 0 008 3z"></path>
</svg>
      <svg title="Search" aria-label="Search" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-search js-jump-to-octicon-search d-none flex-shrink-0">
    <path fill-rule="evenodd" d="M11.5 7a4.499 4.499 0 11-8.998 0A4.499 4.499 0 0111.5 7zm-.82 4.74a6 6 0 111.06-1.06l3.04 3.04a.75.75 0 11-1.06 1.06l-3.04-3.04z"></path>
</svg>
    </div>

    <img class="avatar mr-2 flex-shrink-0 js-jump-to-suggestion-avatar d-none" alt="" aria-label="Team" src="" width="28" height="28">

    <div class="jump-to-suggestion-name js-jump-to-suggestion-name flex-auto overflow-hidden text-left no-wrap css-truncate css-truncate-target">
    </div>

    <div class="border rounded-2 flex-shrink-0 color-bg-subtle px-1 color-fg-muted ml-1 f6 d-none js-jump-to-badge-search">
      <span class="js-jump-to-badge-search-text-default d-none" aria-label="in this repository">
        In this repository
      </span>
      <span class="js-jump-to-badge-search-text-global d-none" aria-label="in all of GitHub">
        All GitHub
      </span>
      <span aria-hidden="true" class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>

    <div aria-hidden="true" class="border rounded-2 flex-shrink-0 color-bg-subtle px-1 color-fg-muted ml-1 f6 d-none d-on-nav-focus js-jump-to-badge-jump">
      Jump to
      <span class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>
  </a>
</li>

</ul>

<ul class="d-none js-jump-to-no-results-template-container">
  <li class="d-flex flex-justify-center flex-items-center f5 d-none js-jump-to-suggestion p-2">
    <span class="color-fg-muted">No suggested jump to results</span>
  </li>
</ul>

<ul id="jump-to-results" role="listbox" class="p-0 m-0 js-navigation-container jump-to-suggestions-results-container js-jump-to-suggestions-results-container">
  

<li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item js-jump-to-scoped-search d-none" role="option">
  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open p-2" href="" data-item-type="scoped_search">
    <div class="jump-to-octicon js-jump-to-octicon flex-shrink-0 mr-2 text-center d-none">
      <svg title="Repository" aria-label="Repository" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-repo js-jump-to-octicon-repo d-none flex-shrink-0">
    <path fill-rule="evenodd" d="M2 2.5A2.5 2.5 0 014.5 0h8.75a.75.75 0 01.75.75v12.5a.75.75 0 01-.75.75h-2.5a.75.75 0 110-1.5h1.75v-2h-8a1 1 0 00-.714 1.7.75.75 0 01-1.072 1.05A2.495 2.495 0 012 11.5v-9zm10.5-1V9h-8c-.356 0-.694.074-1 .208V2.5a1 1 0 011-1h8zM5 12.25v3.25a.25.25 0 00.4.2l1.45-1.087a.25.25 0 01.3 0L8.6 15.7a.25.25 0 00.4-.2v-3.25a.25.25 0 00-.25-.25h-3.5a.25.25 0 00-.25.25z"></path>
</svg>
      <svg title="Project" aria-label="Project" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-project js-jump-to-octicon-project d-none flex-shrink-0">
    <path fill-rule="evenodd" d="M1.75 0A1.75 1.75 0 000 1.75v12.5C0 15.216.784 16 1.75 16h12.5A1.75 1.75 0 0016 14.25V1.75A1.75 1.75 0 0014.25 0H1.75zM1.5 1.75a.25.25 0 01.25-.25h12.5a.25.25 0 01.25.25v12.5a.25.25 0 01-.25.25H1.75a.25.25 0 01-.25-.25V1.75zM11.75 3a.75.75 0 00-.75.75v7.5a.75.75 0 001.5 0v-7.5a.75.75 0 00-.75-.75zm-8.25.75a.75.75 0 011.5 0v5.5a.75.75 0 01-1.5 0v-5.5zM8 3a.75.75 0 00-.75.75v3.5a.75.75 0 001.5 0v-3.5A.75.75 0 008 3z"></path>
</svg>
      <svg title="Search" aria-label="Search" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-search js-jump-to-octicon-search d-none flex-shrink-0">
    <path fill-rule="evenodd" d="M11.5 7a4.499 4.499 0 11-8.998 0A4.499 4.499 0 0111.5 7zm-.82 4.74a6 6 0 111.06-1.06l3.04 3.04a.75.75 0 11-1.06 1.06l-3.04-3.04z"></path>
</svg>
    </div>

    <img class="avatar mr-2 flex-shrink-0 js-jump-to-suggestion-avatar d-none" alt="" aria-label="Team" src="" width="28" height="28">

    <div class="jump-to-suggestion-name js-jump-to-suggestion-name flex-auto overflow-hidden text-left no-wrap css-truncate css-truncate-target">
    </div>

    <div class="border rounded-2 flex-shrink-0 color-bg-subtle px-1 color-fg-muted ml-1 f6 d-none js-jump-to-badge-search">
      <span class="js-jump-to-badge-search-text-default d-none" aria-label="in this repository">
        In this repository
      </span>
      <span class="js-jump-to-badge-search-text-global d-none" aria-label="in all of GitHub">
        All GitHub
      </span>
      <span aria-hidden="true" class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>

    <div aria-hidden="true" class="border rounded-2 flex-shrink-0 color-bg-subtle px-1 color-fg-muted ml-1 f6 d-none d-on-nav-focus js-jump-to-badge-jump">
      Jump to
      <span class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>
  </a>
</li>

  

<li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item js-jump-to-owner-scoped-search d-none" role="option">
  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open p-2" href="" data-item-type="owner_scoped_search">
    <div class="jump-to-octicon js-jump-to-octicon flex-shrink-0 mr-2 text-center d-none">
      <svg title="Repository" aria-label="Repository" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-repo js-jump-to-octicon-repo d-none flex-shrink-0">
    <path fill-rule="evenodd" d="M2 2.5A2.5 2.5 0 014.5 0h8.75a.75.75 0 01.75.75v12.5a.75.75 0 01-.75.75h-2.5a.75.75 0 110-1.5h1.75v-2h-8a1 1 0 00-.714 1.7.75.75 0 01-1.072 1.05A2.495 2.495 0 012 11.5v-9zm10.5-1V9h-8c-.356 0-.694.074-1 .208V2.5a1 1 0 011-1h8zM5 12.25v3.25a.25.25 0 00.4.2l1.45-1.087a.25.25 0 01.3 0L8.6 15.7a.25.25 0 00.4-.2v-3.25a.25.25 0 00-.25-.25h-3.5a.25.25 0 00-.25.25z"></path>
</svg>
      <svg title="Project" aria-label="Project" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-project js-jump-to-octicon-project d-none flex-shrink-0">
    <path fill-rule="evenodd" d="M1.75 0A1.75 1.75 0 000 1.75v12.5C0 15.216.784 16 1.75 16h12.5A1.75 1.75 0 0016 14.25V1.75A1.75 1.75 0 0014.25 0H1.75zM1.5 1.75a.25.25 0 01.25-.25h12.5a.25.25 0 01.25.25v12.5a.25.25 0 01-.25.25H1.75a.25.25 0 01-.25-.25V1.75zM11.75 3a.75.75 0 00-.75.75v7.5a.75.75 0 001.5 0v-7.5a.75.75 0 00-.75-.75zm-8.25.75a.75.75 0 011.5 0v5.5a.75.75 0 01-1.5 0v-5.5zM8 3a.75.75 0 00-.75.75v3.5a.75.75 0 001.5 0v-3.5A.75.75 0 008 3z"></path>
</svg>
      <svg title="Search" aria-label="Search" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-search js-jump-to-octicon-search d-none flex-shrink-0">
    <path fill-rule="evenodd" d="M11.5 7a4.499 4.499 0 11-8.998 0A4.499 4.499 0 0111.5 7zm-.82 4.74a6 6 0 111.06-1.06l3.04 3.04a.75.75 0 11-1.06 1.06l-3.04-3.04z"></path>
</svg>
    </div>

    <img class="avatar mr-2 flex-shrink-0 js-jump-to-suggestion-avatar d-none" alt="" aria-label="Team" src="" width="28" height="28">

    <div class="jump-to-suggestion-name js-jump-to-suggestion-name flex-auto overflow-hidden text-left no-wrap css-truncate css-truncate-target">
    </div>

    <div class="border rounded-2 flex-shrink-0 color-bg-subtle px-1 color-fg-muted ml-1 f6 d-none js-jump-to-badge-search">
      <span class="js-jump-to-badge-search-text-default d-none" aria-label="in this user">
        In this user
      </span>
      <span class="js-jump-to-badge-search-text-global d-none" aria-label="in all of GitHub">
        All GitHub
      </span>
      <span aria-hidden="true" class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>

    <div aria-hidden="true" class="border rounded-2 flex-shrink-0 color-bg-subtle px-1 color-fg-muted ml-1 f6 d-none d-on-nav-focus js-jump-to-badge-jump">
      Jump to
      <span class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>
  </a>
</li>

  

<li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item js-jump-to-global-search d-none" role="option">
  <a tabindex="-1" class="no-underline d-flex flex-auto flex-items-center jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open p-2" href="" data-item-type="global_search">
    <div class="jump-to-octicon js-jump-to-octicon flex-shrink-0 mr-2 text-center d-none">
      <svg title="Repository" aria-label="Repository" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-repo js-jump-to-octicon-repo d-none flex-shrink-0">
    <path fill-rule="evenodd" d="M2 2.5A2.5 2.5 0 014.5 0h8.75a.75.75 0 01.75.75v12.5a.75.75 0 01-.75.75h-2.5a.75.75 0 110-1.5h1.75v-2h-8a1 1 0 00-.714 1.7.75.75 0 01-1.072 1.05A2.495 2.495 0 012 11.5v-9zm10.5-1V9h-8c-.356 0-.694.074-1 .208V2.5a1 1 0 011-1h8zM5 12.25v3.25a.25.25 0 00.4.2l1.45-1.087a.25.25 0 01.3 0L8.6 15.7a.25.25 0 00.4-.2v-3.25a.25.25 0 00-.25-.25h-3.5a.25.25 0 00-.25.25z"></path>
</svg>
      <svg title="Project" aria-label="Project" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-project js-jump-to-octicon-project d-none flex-shrink-0">
    <path fill-rule="evenodd" d="M1.75 0A1.75 1.75 0 000 1.75v12.5C0 15.216.784 16 1.75 16h12.5A1.75 1.75 0 0016 14.25V1.75A1.75 1.75 0 0014.25 0H1.75zM1.5 1.75a.25.25 0 01.25-.25h12.5a.25.25 0 01.25.25v12.5a.25.25 0 01-.25.25H1.75a.25.25 0 01-.25-.25V1.75zM11.75 3a.75.75 0 00-.75.75v7.5a.75.75 0 001.5 0v-7.5a.75.75 0 00-.75-.75zm-8.25.75a.75.75 0 011.5 0v5.5a.75.75 0 01-1.5 0v-5.5zM8 3a.75.75 0 00-.75.75v3.5a.75.75 0 001.5 0v-3.5A.75.75 0 008 3z"></path>
</svg>
      <svg title="Search" aria-label="Search" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-search js-jump-to-octicon-search d-none flex-shrink-0">
    <path fill-rule="evenodd" d="M11.5 7a4.499 4.499 0 11-8.998 0A4.499 4.499 0 0111.5 7zm-.82 4.74a6 6 0 111.06-1.06l3.04 3.04a.75.75 0 11-1.06 1.06l-3.04-3.04z"></path>
</svg>
    </div>

    <img class="avatar mr-2 flex-shrink-0 js-jump-to-suggestion-avatar d-none" alt="" aria-label="Team" src="" width="28" height="28">

    <div class="jump-to-suggestion-name js-jump-to-suggestion-name flex-auto overflow-hidden text-left no-wrap css-truncate css-truncate-target">
    </div>

    <div class="border rounded-2 flex-shrink-0 color-bg-subtle px-1 color-fg-muted ml-1 f6 d-none js-jump-to-badge-search">
      <span class="js-jump-to-badge-search-text-default d-none" aria-label="in this repository">
        In this repository
      </span>
      <span class="js-jump-to-badge-search-text-global d-none" aria-label="in all of GitHub">
        All GitHub
      </span>
      <span aria-hidden="true" class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>

    <div aria-hidden="true" class="border rounded-2 flex-shrink-0 color-bg-subtle px-1 color-fg-muted ml-1 f6 d-none d-on-nav-focus js-jump-to-badge-jump">
      Jump to
      <span class="d-inline-block ml-1 v-align-middle">↵</span>
    </div>
  </a>
</li>


    <li class="d-flex flex-justify-center flex-items-center p-0 f5 js-jump-to-suggestion">
      <svg style="box-sizing: content-box; color: var(--color-icon-primary);" width="32" height="32" viewBox="0 0 16 16" fill="none" data-view-component="true" class="m-3 anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" />
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke" />
</svg>
    </li>
</ul>

          </div>
      </label>
</form>  </div>
</div>

        <nav id="global-nav" class="d-flex flex-column flex-md-row flex-self-stretch flex-md-self-auto" aria-label="Global">
    <a class="Header-link py-md-3 d-block d-md-none py-2 border-top border-md-top-0 border-white-fade" data-ga-click="Header, click, Nav menu - item:dashboard:user" aria-label="Dashboard" data-turbo="false" href="/dashboard">Dashboard</a>

  <a class="js-selected-navigation-item Header-link mt-md-n3 mb-md-n3 py-2 py-md-3 mr-0 mr-md-3 border-top border-md-top-0 border-white-fade" data-hotkey="g p" data-ga-click="Header, click, Nav menu - item:pulls context:user" aria-label="Pull requests you created" data-turbo="false" data-selected-links="/pulls /pulls/assigned /pulls/mentioned /pulls" href="/pulls">
      Pull<span class="d-inline d-md-none d-lg-inline"> request</span>s
</a>
  <a class="js-selected-navigation-item Header-link mt-md-n3 mb-md-n3 py-2 py-md-3 mr-0 mr-md-3 border-top border-md-top-0 border-white-fade" data-hotkey="g i" data-ga-click="Header, click, Nav menu - item:issues context:user" aria-label="Issues you created" data-turbo="false" data-selected-links="/issues /issues/assigned /issues/mentioned /issues" href="/issues">Issues</a>

    <a class="js-selected-navigation-item Header-link mt-md-n3 mb-md-n3 py-2 py-md-3 mr-0 mr-md-3 border-top border-md-top-0 border-white-fade" data-ga-click="Header, click, Nav menu - item:workspaces context:user" data-turbo="false" data-selected-links="/codespaces /codespaces" href="/codespaces">Codespaces</a>

    <div class="d-flex position-relative">
      <a class="js-selected-navigation-item Header-link flex-auto mt-md-n3 mb-md-n3 py-2 py-md-3 mr-0 mr-md-3 border-top border-md-top-0 border-white-fade" data-ga-click="Header, click, Nav menu - item:marketplace context:user" data-octo-click="marketplace_click" data-octo-dimensions="location:nav_bar" data-turbo="false" data-selected-links=" /marketplace" href="/marketplace">Marketplace</a>
    </div>

  <a class="js-selected-navigation-item Header-link mt-md-n3 mb-md-n3 py-2 py-md-3 mr-0 mr-md-3 border-top border-md-top-0 border-white-fade" data-ga-click="Header, click, Nav menu - item:explore" data-turbo="false" data-selected-links="/explore /trending /trending/developers /integrations /integrations/feature/code /integrations/feature/collaborate /integrations/feature/ship showcases showcases_search showcases_landing /explore" href="/explore">Explore</a>

      <a class="js-selected-navigation-item Header-link d-block d-md-none py-2 py-md-3 border-top border-md-top-0 border-white-fade" data-ga-click="Header, click, Nav menu - item:Sponsors" data-hydro-click="{&quot;event_type&quot;:&quot;sponsors.button_click&quot;,&quot;payload&quot;:{&quot;button&quot;:&quot;HEADER_SPONSORS_DASHBOARD&quot;,&quot;sponsorable_login&quot;:&quot;sean207cc&quot;,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="0a4d7e073c3ac5a6743e4983122ab286610a262aa7bb1e6d8e5bb8c86a337d24" data-turbo="false" data-selected-links=" /sponsors/accounts" href="/sponsors/accounts">Sponsors</a>

    <a class="Header-link d-block d-md-none mr-0 mr-md-3 py-2 py-md-3 border-top border-md-top-0 border-white-fade" data-turbo="false" href="/settings/profile">Settings</a>

    <a class="Header-link d-block d-md-none mr-0 mr-md-3 py-2 py-md-3 border-top border-md-top-0 border-white-fade" data-turbo="false" href="/sean207cc">
      <img class="avatar avatar-user" loading="lazy" decoding="async" src="https://avatars.githubusercontent.com/u/114159512?s=40&amp;v=4" width="20" height="20" alt="@sean207cc" />
      sean207cc
</a>
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form data-turbo="false" action="/logout" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="5sWV6_lXvixWBgkQaRBg57EbcIXQJPDngbqyJIs25MFZkGdBNue-IrgX8Q6pkwgWW6r53kuZTa35Z8leVm7NmQ" />
      <button
        type="submit"
        class="Header-link mr-0 mr-md-3 py-2 py-md-3 border-top border-md-top-0 border-white-fade d-md-none btn-link d-block width-full text-left"
        style="padding-left: 2px;"
        data-analytics-event="{&quot;category&quot;:&quot;Header&quot;,&quot;action&quot;:&quot;sign out&quot;,&quot;label&quot;:&quot;icon:logout&quot;}"
      >
        <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-sign-out v-align-middle">
    <path fill-rule="evenodd" d="M2 2.75C2 1.784 2.784 1 3.75 1h2.5a.75.75 0 010 1.5h-2.5a.25.25 0 00-.25.25v10.5c0 .138.112.25.25.25h2.5a.75.75 0 010 1.5h-2.5A1.75 1.75 0 012 13.25V2.75zm10.44 4.5H6.75a.75.75 0 000 1.5h5.69l-1.97 1.97a.75.75 0 101.06 1.06l3.25-3.25a.75.75 0 000-1.06l-3.25-3.25a.75.75 0 10-1.06 1.06l1.97 1.97z"></path>
</svg>
        Sign out
      </button>
</form></nav>

    </div>

    <div class="Header-item Header-item--full flex-justify-center d-md-none position-relative">
        <a
  class="Header-link"
  href="https://github.com/"
  data-hotkey="g d"
  aria-label="Homepage "
  data-turbo="false"
  data-analytics-event="{&quot;category&quot;:&quot;Header&quot;,&quot;action&quot;:&quot;go to dashboard&quot;,&quot;label&quot;:&quot;icon:logo&quot;}"
>
  <svg height="32" aria-hidden="true" viewBox="0 0 16 16" version="1.1" width="32" data-view-component="true" class="octicon octicon-mark-github v-align-middle">
    <path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path>
</svg>
</a>

    </div>

    <div class="Header-item mr-0 mr-md-3 flex-order-1 flex-md-order-none">
        

<notification-indicator data-channel="eyJjIjoibm90aWZpY2F0aW9uLWNoYW5nZWQ6MTE0MTU5NTEyIiwidCI6MTY3MDQ5OTUzM30=--38d344bb3b388d6aca5d6a4aa3aba1deb37badd7929ca3f787682e50d6b6f128" data-indicator-mode="global" data-tooltip-global="You have unread notifications" data-tooltip-unavailable="Notifications are unavailable at the moment." data-tooltip-none="You have no unread notifications" data-view-component="true" class="js-socket-channel">
  <a id="AppHeader-notifications-button" href="/notifications"
    class="Header-link notification-indicator position-relative tooltipped tooltipped-sw"

    

    data-hotkey="g n"
    data-target="notification-indicator.link"
    aria-label="Notifications"

      data-analytics-event="{&quot;category&quot;:&quot;Header&quot;,&quot;action&quot;:&quot;go to notifications&quot;,&quot;label&quot;:&quot;icon:unread&quot;}"
  >

    <span
      data-target="notification-indicator.badge"
      class="mail-status unread" >
    </span>

      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-bell">
    <path d="M8 16a2 2 0 001.985-1.75c.017-.137-.097-.25-.235-.25h-3.5c-.138 0-.252.113-.235.25A2 2 0 008 16z"></path><path fill-rule="evenodd" d="M8 1.5A3.5 3.5 0 004.5 5v2.947c0 .346-.102.683-.294.97l-1.703 2.556a.018.018 0 00-.003.01l.001.006c0 .002.002.004.004.006a.017.017 0 00.006.004l.007.001h10.964l.007-.001a.016.016 0 00.006-.004.016.016 0 00.004-.006l.001-.007a.017.017 0 00-.003-.01l-1.703-2.554a1.75 1.75 0 01-.294-.97V5A3.5 3.5 0 008 1.5zM3 5a5 5 0 0110 0v2.947c0 .05.015.098.042.139l1.703 2.555A1.518 1.518 0 0113.482 13H2.518a1.518 1.518 0 01-1.263-2.36l1.703-2.554A.25.25 0 003 7.947V5z"></path>
</svg>
  </a>

</notification-indicator>
    </div>


    <div class="Header-item position-relative d-none d-md-flex">
        <details class="details-overlay details-reset">
  <summary
    class="Header-link"
    aria-label="Create new…"
    data-analytics-event="{&quot;category&quot;:&quot;Header&quot;,&quot;action&quot;:&quot;create new&quot;,&quot;label&quot;:&quot;icon:add&quot;}"
  >
    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-plus">
    <path fill-rule="evenodd" d="M7.75 2a.75.75 0 01.75.75V7h4.25a.75.75 0 110 1.5H8.5v4.25a.75.75 0 11-1.5 0V8.5H2.75a.75.75 0 010-1.5H7V2.75A.75.75 0 017.75 2z"></path>
</svg> <span class="dropdown-caret"></span>
  </summary>
  <details-menu class="dropdown-menu dropdown-menu-sw">
    
<a role="menuitem" class="dropdown-item" href="/new" data-ga-click="Header, create new repository">
  New repository
</a>

  <a role="menuitem" class="dropdown-item" href="/new/import" data-ga-click="Header, import a repository">
    Import repository
  </a>

<a role="menuitem" class="dropdown-item" href="/codespaces/new">
  New codespace
</a>

<a role="menuitem" class="dropdown-item" href="https://gist.github.com/" data-ga-click="Header, create new gist">
  New gist
</a>

  <a role="menuitem" class="dropdown-item" href="/organizations/new" data-ga-click="Header, create new organization">
    New organization
  </a>



  </details-menu>
</details>

    </div>

    <div class="Header-item position-relative mr-0 d-none d-md-flex">
        
  <details class="details-overlay details-reset js-feature-preview-indicator-container" data-feature-preview-indicator-src="/users/sean207cc/feature_preview/indicator_check">

  <summary
    class="Header-link"
    aria-label="View profile and more"
    data-analytics-event="{&quot;category&quot;:&quot;Header&quot;,&quot;action&quot;:&quot;show menu&quot;,&quot;label&quot;:&quot;icon:avatar&quot;}"
  >
    <img src="https://avatars.githubusercontent.com/u/114159512?s=40&amp;v=4" alt="@sean207cc" size="20" height="20" width="20" data-view-component="true" class="avatar avatar-small circle" />
      <span class="unread-indicator js-feature-preview-indicator" style="top: 1px;" hidden></span>
    <span class="dropdown-caret"></span>
  </summary>
  <details-menu
      class="dropdown-menu dropdown-menu-sw"
      style="width: 180px"
      
      preload>
      <include-fragment src="/users/114159512/menu" loading="lazy">
        <p class="text-center mt-3" data-hide-on-error>
          <svg style="box-sizing: content-box; color: var(--color-icon-primary);" width="32" height="32" viewBox="0 0 16 16" fill="none" data-view-component="true" class="anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" />
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke" />
</svg>
        </p>
        <p class="ml-1 mb-2 mt-2 color-fg-default" data-show-on-error>
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-alert">
    <path fill-rule="evenodd" d="M8.22 1.754a.25.25 0 00-.44 0L1.698 13.132a.25.25 0 00.22.368h12.164a.25.25 0 00.22-.368L8.22 1.754zm-1.763-.707c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0114.082 15H1.918a1.75 1.75 0 01-1.543-2.575L6.457 1.047zM9 11a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.25a.75.75 0 00-1.5 0v2.5a.75.75 0 001.5 0v-2.5z"></path>
</svg>
          Sorry, something went wrong.
        </p>
      </include-fragment>
  </details-menu>
</details>

    </div>

</header>

            
    </div>

  <div id="start-of-content" class="show-on-focus"></div>







    <div id="js-flash-container" data-turbo-replace>




  <template class="js-flash-template">
    
<div class="flash flash-full   {{ className }}">
  <div class="px-2" >
    <button autofocus class="flash-close js-flash-close" type="button" aria-label="Dismiss this message">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path>
</svg>
    </button>
    <div aria-atomic="true" role="alert" class="js-flash-alert">
      
      <div>{{ message }}</div>

    </div>
  </div>
</div>
  </template>
</div>


    
  <include-fragment class="js-notification-shelf-include-fragment" data-base-src="https://github.com/notifications/beta/shelf"></include-fragment>





      <details
  class="details-reset details-overlay details-overlay-dark js-command-palette-dialog"
  id="command-palette-pjax-container"
  data-turbo-replace
>
  <summary aria-label="command palette trigger" tabindex="-1"></summary>
  <details-dialog class="command-palette-details-dialog d-flex flex-column flex-justify-center height-fit" aria-label="command palette">
    <command-palette
      class="command-palette color-bg-default rounded-3 border color-shadow-small"
      return-to=/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md
      user-id="114159512"
      activation-hotkey="Mod+k,Mod+Alt+k"
      command-mode-hotkey="Mod+Shift+k"
      data-action="
        command-palette-input-ready:command-palette#inputReady
        command-palette-page-stack-updated:command-palette#updateInputScope
        itemsUpdated:command-palette#itemsUpdated
        keydown:command-palette#onKeydown
        loadingStateChanged:command-palette#loadingStateChanged
        selectedItemChanged:command-palette#selectedItemChanged
        pageFetchError:command-palette#pageFetchError
      ">

        <command-palette-mode
          data-char="#"
            data-scope-types="[&quot;&quot;]"
            data-placeholder="Search issues and pull requests"
        ></command-palette-mode>
        <command-palette-mode
          data-char="#"
            data-scope-types="[&quot;owner&quot;,&quot;repository&quot;]"
            data-placeholder="Search issues, pull requests, discussions, and projects"
        ></command-palette-mode>
        <command-palette-mode
          data-char="!"
            data-scope-types="[&quot;owner&quot;,&quot;repository&quot;]"
            data-placeholder="Search projects"
        ></command-palette-mode>
        <command-palette-mode
          data-char="@"
            data-scope-types="[&quot;&quot;]"
            data-placeholder="Search or jump to a user, organization, or repository"
        ></command-palette-mode>
        <command-palette-mode
          data-char="@"
            data-scope-types="[&quot;owner&quot;]"
            data-placeholder="Search or jump to a repository"
        ></command-palette-mode>
        <command-palette-mode
          data-char="/"
            data-scope-types="[&quot;repository&quot;]"
            data-placeholder="Search files"
        ></command-palette-mode>
        <command-palette-mode
          data-char="?"
        ></command-palette-mode>
        <command-palette-mode
          data-char="&gt;"
            data-placeholder="Run a command"
        ></command-palette-mode>
        <command-palette-mode
          data-char=""
            data-scope-types="[&quot;&quot;]"
            data-placeholder="Search or jump to..."
        ></command-palette-mode>
        <command-palette-mode
          data-char=""
            data-scope-types="[&quot;owner&quot;]"
            data-placeholder="Search or jump to..."
        ></command-palette-mode>
      <command-palette-mode
        class="js-command-palette-default-mode"
        data-char=""
        data-placeholder="Search or jump to..."
      ></command-palette-mode>

      <command-palette-input placeholder="Search or jump to..."

        data-action="
          command-palette-input:command-palette#onInput
          command-palette-select:command-palette#onSelect
          command-palette-descope:command-palette#onDescope
          command-palette-cleared:command-palette#onInputClear
        "
      >
        <div class="js-search-icon d-flex flex-items-center mr-2" style="height: 26px">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-search color-fg-muted">
    <path fill-rule="evenodd" d="M11.5 7a4.499 4.499 0 11-8.998 0A4.499 4.499 0 0111.5 7zm-.82 4.74a6 6 0 111.06-1.06l3.04 3.04a.75.75 0 11-1.06 1.06l-3.04-3.04z"></path>
</svg>
        </div>
        <div class="js-spinner d-flex flex-items-center mr-2 color-fg-muted" hidden>
          <svg aria-label="Loading" class="anim-rotate" viewBox="0 0 16 16" fill="none" width="16" height="16">
            <circle
              cx="8"
              cy="8"
              r="7"
              stroke="currentColor"
              stroke-opacity="0.25"
              stroke-width="2"
              vector-effect="non-scaling-stroke"
            ></circle>
            <path
              d="M15 8a7.002 7.002 0 00-7-7"
              stroke="currentColor"
              stroke-width="2"
              stroke-linecap="round"
              vector-effect="non-scaling-stroke"
            ></path>
          </svg>
        </div>
        <command-palette-scope >
          <div data-target="command-palette-scope.placeholder" hidden class="color-fg-subtle">/&nbsp;&nbsp;<span class="text-semibold color-fg-default">...</span>&nbsp;&nbsp;/&nbsp;&nbsp;</div>
              <command-palette-token
                data-text="sean207cc"
                data-id="U_kgDOBs3vmA"
                data-type="owner"
                data-value="sean207cc"
                data-targets="command-palette-scope.tokens"
                class="color-fg-default text-semibold"
                style="white-space:nowrap;line-height:20px;"
                >sean207cc<span class="color-fg-subtle text-normal">&nbsp;&nbsp;/&nbsp;&nbsp;</span></command-palette-token>
              <command-palette-token
                data-text="AI-course"
                data-id="R_kgDOIlI2oQ"
                data-type="repository"
                data-value="AI-course"
                data-targets="command-palette-scope.tokens"
                class="color-fg-default text-semibold"
                style="white-space:nowrap;line-height:20px;"
                >AI-course<span class="color-fg-subtle text-normal">&nbsp;&nbsp;/&nbsp;&nbsp;</span></command-palette-token>
        </command-palette-scope>
        <div class="command-palette-input-group flex-1 form-control border-0 box-shadow-none" style="z-index: 0">
          <div class="command-palette-typeahead position-absolute d-flex flex-items-center Truncate">
            <span class="typeahead-segment input-mirror" data-target="command-palette-input.mirror"></span>
            <span class="Truncate-text" data-target="command-palette-input.typeaheadText"></span>
            <span class="typeahead-segment" data-target="command-palette-input.typeaheadPlaceholder"></span>
          </div>
          <input
            class="js-overlay-input typeahead-input d-none"
            disabled
            tabindex="-1"
            aria-label="Hidden input for typeahead"
          >
          <input
            type="text"
            autocomplete="off"
            autocorrect="off"
            autocapitalize="off"
            spellcheck="false"
            class="js-input typeahead-input form-control border-0 box-shadow-none input-block width-full no-focus-indicator"
            aria-label="Command palette input"
            aria-haspopup="listbox"
            aria-expanded="false"
            aria-autocomplete="list"
            aria-controls="command-palette-page-stack"
            role="combobox"
            data-action="
              input:command-palette-input#onInput
              keydown:command-palette-input#onKeydown
            "
          >
        </div>
          <div data-view-component="true" class="position-relative d-inline-block">
    <button aria-keyshortcuts="Meta+Delete" data-action="click:command-palette-input#onClear keypress:command-palette-input#onClear" data-target="command-palette-input.clearButton" id="command-palette-clear-button" hidden="hidden" type="button" data-view-component="true" class="btn-octicon command-palette-input-clear-button">      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x-circle-fill">
    <path fill-rule="evenodd" d="M2.343 13.657A8 8 0 1113.657 2.343 8 8 0 012.343 13.657zM6.03 4.97a.75.75 0 00-1.06 1.06L6.94 8 4.97 9.97a.75.75 0 101.06 1.06L8 9.06l1.97 1.97a.75.75 0 101.06-1.06L9.06 8l1.97-1.97a.75.75 0 10-1.06-1.06L8 6.94 6.03 4.97z"></path>
</svg>
</button>    <tool-tip for="command-palette-clear-button" data-direction="w" data-type="label" data-view-component="true" class="sr-only position-absolute">Clear Command Palette</tool-tip>
</div>
      </command-palette-input>

      <command-palette-page-stack
        data-default-scope-id="R_kgDOIlI2oQ"
        data-default-scope-type="Repository"
        data-action="command-palette-page-octicons-cached:command-palette-page-stack#cacheOcticons"
      >
          <command-palette-tip
            class="color-fg-muted f6 px-3 py-1 my-2"
              data-scope-types="[&quot;&quot;,&quot;owner&quot;,&quot;repository&quot;]"
            data-mode=""
            data-value="">
            <div class="d-flex flex-items-start flex-justify-between">
              <div>
                <span class="text-bold">Tip:</span>
                  Type <kbd class="hx_kbd">#</kbd> to search pull requests
              </div>
              <div class="ml-2 flex-shrink-0">
                Type <kbd class="hx_kbd">?</kbd> for help and tips
              </div>
            </div>
          </command-palette-tip>
          <command-palette-tip
            class="color-fg-muted f6 px-3 py-1 my-2"
              data-scope-types="[&quot;&quot;,&quot;owner&quot;,&quot;repository&quot;]"
            data-mode=""
            data-value="">
            <div class="d-flex flex-items-start flex-justify-between">
              <div>
                <span class="text-bold">Tip:</span>
                  Type <kbd class="hx_kbd">#</kbd> to search issues
              </div>
              <div class="ml-2 flex-shrink-0">
                Type <kbd class="hx_kbd">?</kbd> for help and tips
              </div>
            </div>
          </command-palette-tip>
          <command-palette-tip
            class="color-fg-muted f6 px-3 py-1 my-2"
              data-scope-types="[&quot;owner&quot;,&quot;repository&quot;]"
            data-mode=""
            data-value="">
            <div class="d-flex flex-items-start flex-justify-between">
              <div>
                <span class="text-bold">Tip:</span>
                  Type <kbd class="hx_kbd">#</kbd> to search discussions
              </div>
              <div class="ml-2 flex-shrink-0">
                Type <kbd class="hx_kbd">?</kbd> for help and tips
              </div>
            </div>
          </command-palette-tip>
          <command-palette-tip
            class="color-fg-muted f6 px-3 py-1 my-2"
              data-scope-types="[&quot;owner&quot;,&quot;repository&quot;]"
            data-mode=""
            data-value="">
            <div class="d-flex flex-items-start flex-justify-between">
              <div>
                <span class="text-bold">Tip:</span>
                  Type <kbd class="hx_kbd">!</kbd> to search projects
              </div>
              <div class="ml-2 flex-shrink-0">
                Type <kbd class="hx_kbd">?</kbd> for help and tips
              </div>
            </div>
          </command-palette-tip>
          <command-palette-tip
            class="color-fg-muted f6 px-3 py-1 my-2"
              data-scope-types="[&quot;owner&quot;]"
            data-mode=""
            data-value="">
            <div class="d-flex flex-items-start flex-justify-between">
              <div>
                <span class="text-bold">Tip:</span>
                  Type <kbd class="hx_kbd">@</kbd> to search teams
              </div>
              <div class="ml-2 flex-shrink-0">
                Type <kbd class="hx_kbd">?</kbd> for help and tips
              </div>
            </div>
          </command-palette-tip>
          <command-palette-tip
            class="color-fg-muted f6 px-3 py-1 my-2"
              data-scope-types="[&quot;&quot;]"
            data-mode=""
            data-value="">
            <div class="d-flex flex-items-start flex-justify-between">
              <div>
                <span class="text-bold">Tip:</span>
                  Type <kbd class="hx_kbd">@</kbd> to search people and organizations
              </div>
              <div class="ml-2 flex-shrink-0">
                Type <kbd class="hx_kbd">?</kbd> for help and tips
              </div>
            </div>
          </command-palette-tip>
          <command-palette-tip
            class="color-fg-muted f6 px-3 py-1 my-2"
              data-scope-types="[&quot;&quot;,&quot;owner&quot;,&quot;repository&quot;]"
            data-mode=""
            data-value="">
            <div class="d-flex flex-items-start flex-justify-between">
              <div>
                <span class="text-bold">Tip:</span>
                  Type <kbd class="hx_kbd">&gt;</kbd> to activate command mode
              </div>
              <div class="ml-2 flex-shrink-0">
                Type <kbd class="hx_kbd">?</kbd> for help and tips
              </div>
            </div>
          </command-palette-tip>
          <command-palette-tip
            class="color-fg-muted f6 px-3 py-1 my-2"
              data-scope-types="[&quot;&quot;,&quot;owner&quot;,&quot;repository&quot;]"
            data-mode=""
            data-value="">
            <div class="d-flex flex-items-start flex-justify-between">
              <div>
                <span class="text-bold">Tip:</span>
                  Go to your accessibility settings to change your keyboard shortcuts
              </div>
              <div class="ml-2 flex-shrink-0">
                Type <kbd class="hx_kbd">?</kbd> for help and tips
              </div>
            </div>
          </command-palette-tip>
          <command-palette-tip
            class="color-fg-muted f6 px-3 py-1 my-2"
              data-scope-types="[&quot;&quot;,&quot;owner&quot;,&quot;repository&quot;]"
            data-mode="#"
            data-value="">
            <div class="d-flex flex-items-start flex-justify-between">
              <div>
                <span class="text-bold">Tip:</span>
                  Type author:@me to search your content
              </div>
              <div class="ml-2 flex-shrink-0">
                Type <kbd class="hx_kbd">?</kbd> for help and tips
              </div>
            </div>
          </command-palette-tip>
          <command-palette-tip
            class="color-fg-muted f6 px-3 py-1 my-2"
              data-scope-types="[&quot;&quot;,&quot;owner&quot;,&quot;repository&quot;]"
            data-mode="#"
            data-value="">
            <div class="d-flex flex-items-start flex-justify-between">
              <div>
                <span class="text-bold">Tip:</span>
                  Type is:pr to filter to pull requests
              </div>
              <div class="ml-2 flex-shrink-0">
                Type <kbd class="hx_kbd">?</kbd> for help and tips
              </div>
            </div>
          </command-palette-tip>
          <command-palette-tip
            class="color-fg-muted f6 px-3 py-1 my-2"
              data-scope-types="[&quot;&quot;,&quot;owner&quot;,&quot;repository&quot;]"
            data-mode="#"
            data-value="">
            <div class="d-flex flex-items-start flex-justify-between">
              <div>
                <span class="text-bold">Tip:</span>
                  Type is:issue to filter to issues
              </div>
              <div class="ml-2 flex-shrink-0">
                Type <kbd class="hx_kbd">?</kbd> for help and tips
              </div>
            </div>
          </command-palette-tip>
          <command-palette-tip
            class="color-fg-muted f6 px-3 py-1 my-2"
              data-scope-types="[&quot;owner&quot;,&quot;repository&quot;]"
            data-mode="#"
            data-value="">
            <div class="d-flex flex-items-start flex-justify-between">
              <div>
                <span class="text-bold">Tip:</span>
                  Type is:project to filter to projects
              </div>
              <div class="ml-2 flex-shrink-0">
                Type <kbd class="hx_kbd">?</kbd> for help and tips
              </div>
            </div>
          </command-palette-tip>
          <command-palette-tip
            class="color-fg-muted f6 px-3 py-1 my-2"
              data-scope-types="[&quot;&quot;,&quot;owner&quot;,&quot;repository&quot;]"
            data-mode="#"
            data-value="">
            <div class="d-flex flex-items-start flex-justify-between">
              <div>
                <span class="text-bold">Tip:</span>
                  Type is:open to filter to open content
              </div>
              <div class="ml-2 flex-shrink-0">
                Type <kbd class="hx_kbd">?</kbd> for help and tips
              </div>
            </div>
          </command-palette-tip>
        <command-palette-tip class="mx-3 my-2 flash flash-error d-flex flex-items-center" data-scope-types="*" data-on-error>
          <div>
            <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-alert">
    <path fill-rule="evenodd" d="M8.22 1.754a.25.25 0 00-.44 0L1.698 13.132a.25.25 0 00.22.368h12.164a.25.25 0 00.22-.368L8.22 1.754zm-1.763-.707c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0114.082 15H1.918a1.75 1.75 0 01-1.543-2.575L6.457 1.047zM9 11a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.25a.75.75 0 00-1.5 0v2.5a.75.75 0 001.5 0v-2.5z"></path>
</svg>
          </div>
          <div class="px-2">
            We’ve encountered an error and some results aren't available at this time. Type a new search or try again later.
          </div>
        </command-palette-tip>
        <command-palette-tip class="h4 color-fg-default pl-3 pb-2 pt-3" data-on-empty data-scope-types="*" data-match-mode="[^?]|^$">
          No results matched your search
        </command-palette-tip>

        <div hidden>

            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="arrow-right-color-fg-muted">
              <svg height="16" class="octicon octicon-arrow-right color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.22 2.97a.75.75 0 011.06 0l4.25 4.25a.75.75 0 010 1.06l-4.25 4.25a.75.75 0 01-1.06-1.06l2.97-2.97H3.75a.75.75 0 010-1.5h7.44L8.22 4.03a.75.75 0 010-1.06z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="arrow-right-color-fg-default">
              <svg height="16" class="octicon octicon-arrow-right color-fg-default" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.22 2.97a.75.75 0 011.06 0l4.25 4.25a.75.75 0 010 1.06l-4.25 4.25a.75.75 0 01-1.06-1.06l2.97-2.97H3.75a.75.75 0 010-1.5h7.44L8.22 4.03a.75.75 0 010-1.06z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="codespaces-color-fg-muted">
              <svg height="16" class="octicon octicon-codespaces color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M2 1.75C2 .784 2.784 0 3.75 0h8.5C13.216 0 14 .784 14 1.75v5a1.75 1.75 0 01-1.75 1.75h-8.5A1.75 1.75 0 012 6.75v-5zm1.75-.25a.25.25 0 00-.25.25v5c0 .138.112.25.25.25h8.5a.25.25 0 00.25-.25v-5a.25.25 0 00-.25-.25h-8.5zM0 11.25c0-.966.784-1.75 1.75-1.75h12.5c.966 0 1.75.784 1.75 1.75v3A1.75 1.75 0 0114.25 16H1.75A1.75 1.75 0 010 14.25v-3zM1.75 11a.25.25 0 00-.25.25v3c0 .138.112.25.25.25h12.5a.25.25 0 00.25-.25v-3a.25.25 0 00-.25-.25H1.75z"></path><path fill-rule="evenodd" d="M3 12.75a.75.75 0 01.75-.75h.5a.75.75 0 010 1.5h-.5a.75.75 0 01-.75-.75zm4 0a.75.75 0 01.75-.75h4.5a.75.75 0 010 1.5h-4.5a.75.75 0 01-.75-.75z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="copy-color-fg-muted">
              <svg height="16" class="octicon octicon-copy color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 010 1.5h-1.5a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-1.5a.75.75 0 011.5 0v1.5A1.75 1.75 0 019.25 16h-7.5A1.75 1.75 0 010 14.25v-7.5z"></path><path fill-rule="evenodd" d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0114.25 11h-7.5A1.75 1.75 0 015 9.25v-7.5zm1.75-.25a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-7.5a.25.25 0 00-.25-.25h-7.5z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="dash-color-fg-muted">
              <svg height="16" class="octicon octicon-dash color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M2 7.75A.75.75 0 012.75 7h10a.75.75 0 010 1.5h-10A.75.75 0 012 7.75z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="file-color-fg-muted">
              <svg height="16" class="octicon octicon-file color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M3.75 1.5a.25.25 0 00-.25.25v12.5c0 .138.112.25.25.25h9.5a.25.25 0 00.25-.25V6h-2.75A1.75 1.75 0 019 4.25V1.5H3.75zm6.75.062V4.25c0 .138.112.25.25.25h2.688a.252.252 0 00-.011-.013l-2.914-2.914a.272.272 0 00-.013-.011zM2 1.75C2 .784 2.784 0 3.75 0h6.586c.464 0 .909.184 1.237.513l2.914 2.914c.329.328.513.773.513 1.237v9.586A1.75 1.75 0 0113.25 16h-9.5A1.75 1.75 0 012 14.25V1.75z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="gear-color-fg-muted">
              <svg height="16" class="octicon octicon-gear color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.429 1.525a6.593 6.593 0 011.142 0c.036.003.108.036.137.146l.289 1.105c.147.56.55.967.997 1.189.174.086.341.183.501.29.417.278.97.423 1.53.27l1.102-.303c.11-.03.175.016.195.046.219.31.41.641.573.989.014.031.022.11-.059.19l-.815.806c-.411.406-.562.957-.53 1.456a4.588 4.588 0 010 .582c-.032.499.119 1.05.53 1.456l.815.806c.08.08.073.159.059.19a6.494 6.494 0 01-.573.99c-.02.029-.086.074-.195.045l-1.103-.303c-.559-.153-1.112-.008-1.529.27-.16.107-.327.204-.5.29-.449.222-.851.628-.998 1.189l-.289 1.105c-.029.11-.101.143-.137.146a6.613 6.613 0 01-1.142 0c-.036-.003-.108-.037-.137-.146l-.289-1.105c-.147-.56-.55-.967-.997-1.189a4.502 4.502 0 01-.501-.29c-.417-.278-.97-.423-1.53-.27l-1.102.303c-.11.03-.175-.016-.195-.046a6.492 6.492 0 01-.573-.989c-.014-.031-.022-.11.059-.19l.815-.806c.411-.406.562-.957.53-1.456a4.587 4.587 0 010-.582c.032-.499-.119-1.05-.53-1.456l-.815-.806c-.08-.08-.073-.159-.059-.19a6.44 6.44 0 01.573-.99c.02-.029.086-.075.195-.045l1.103.303c.559.153 1.112.008 1.529-.27.16-.107.327-.204.5-.29.449-.222.851-.628.998-1.189l.289-1.105c.029-.11.101-.143.137-.146zM8 0c-.236 0-.47.01-.701.03-.743.065-1.29.615-1.458 1.261l-.29 1.106c-.017.066-.078.158-.211.224a5.994 5.994 0 00-.668.386c-.123.082-.233.09-.3.071L3.27 2.776c-.644-.177-1.392.02-1.82.63a7.977 7.977 0 00-.704 1.217c-.315.675-.111 1.422.363 1.891l.815.806c.05.048.098.147.088.294a6.084 6.084 0 000 .772c.01.147-.038.246-.088.294l-.815.806c-.474.469-.678 1.216-.363 1.891.2.428.436.835.704 1.218.428.609 1.176.806 1.82.63l1.103-.303c.066-.019.176-.011.299.071.213.143.436.272.668.386.133.066.194.158.212.224l.289 1.106c.169.646.715 1.196 1.458 1.26a8.094 8.094 0 001.402 0c.743-.064 1.29-.614 1.458-1.26l.29-1.106c.017-.066.078-.158.211-.224a5.98 5.98 0 00.668-.386c.123-.082.233-.09.3-.071l1.102.302c.644.177 1.392-.02 1.82-.63.268-.382.505-.789.704-1.217.315-.675.111-1.422-.364-1.891l-.814-.806c-.05-.048-.098-.147-.088-.294a6.1 6.1 0 000-.772c-.01-.147.039-.246.088-.294l.814-.806c.475-.469.679-1.216.364-1.891a7.992 7.992 0 00-.704-1.218c-.428-.609-1.176-.806-1.82-.63l-1.103.303c-.066.019-.176.011-.299-.071a5.991 5.991 0 00-.668-.386c-.133-.066-.194-.158-.212-.224L10.16 1.29C9.99.645 9.444.095 8.701.031A8.094 8.094 0 008 0zm1.5 8a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0zM11 8a3 3 0 11-6 0 3 3 0 016 0z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="lock-color-fg-muted">
              <svg height="16" class="octicon octicon-lock color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 4v2h-.25A1.75 1.75 0 002 7.75v5.5c0 .966.784 1.75 1.75 1.75h8.5A1.75 1.75 0 0014 13.25v-5.5A1.75 1.75 0 0012.25 6H12V4a4 4 0 10-8 0zm6.5 2V4a2.5 2.5 0 00-5 0v2h5zM12 7.5h.25a.25.25 0 01.25.25v5.5a.25.25 0 01-.25.25h-8.5a.25.25 0 01-.25-.25v-5.5a.25.25 0 01.25-.25H12z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="moon-color-fg-muted">
              <svg height="16" class="octicon octicon-moon color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M9.598 1.591a.75.75 0 01.785-.175 7 7 0 11-8.967 8.967.75.75 0 01.961-.96 5.5 5.5 0 007.046-7.046.75.75 0 01.175-.786zm1.616 1.945a7 7 0 01-7.678 7.678 5.5 5.5 0 107.678-7.678z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="person-color-fg-muted">
              <svg height="16" class="octicon octicon-person color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M10.5 5a2.5 2.5 0 11-5 0 2.5 2.5 0 015 0zm.061 3.073a4 4 0 10-5.123 0 6.004 6.004 0 00-3.431 5.142.75.75 0 001.498.07 4.5 4.5 0 018.99 0 .75.75 0 101.498-.07 6.005 6.005 0 00-3.432-5.142z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="pencil-color-fg-muted">
              <svg height="16" class="octicon octicon-pencil color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M11.013 1.427a1.75 1.75 0 012.474 0l1.086 1.086a1.75 1.75 0 010 2.474l-8.61 8.61c-.21.21-.47.364-.756.445l-3.251.93a.75.75 0 01-.927-.928l.929-3.25a1.75 1.75 0 01.445-.758l8.61-8.61zm1.414 1.06a.25.25 0 00-.354 0L10.811 3.75l1.439 1.44 1.263-1.263a.25.25 0 000-.354l-1.086-1.086zM11.189 6.25L9.75 4.81l-6.286 6.287a.25.25 0 00-.064.108l-.558 1.953 1.953-.558a.249.249 0 00.108-.064l6.286-6.286z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="issue-opened-open">
              <svg height="16" class="octicon octicon-issue-opened open" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path d="M8 9.5a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path><path fill-rule="evenodd" d="M8 0a8 8 0 100 16A8 8 0 008 0zM1.5 8a6.5 6.5 0 1113 0 6.5 6.5 0 01-13 0z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="git-pull-request-draft-color-fg-muted">
              <svg height="16" class="octicon octicon-git-pull-request-draft color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M2.5 3.25a.75.75 0 111.5 0 .75.75 0 01-1.5 0zM3.25 1a2.25 2.25 0 00-.75 4.372v5.256a2.251 2.251 0 101.5 0V5.372A2.25 2.25 0 003.25 1zm0 11a.75.75 0 100 1.5.75.75 0 000-1.5zm9.5 3a2.25 2.25 0 100-4.5 2.25 2.25 0 000 4.5zm0-3a.75.75 0 100 1.5.75.75 0 000-1.5z"></path><path d="M14 7.5a1.25 1.25 0 11-2.5 0 1.25 1.25 0 012.5 0zm0-4.25a1.25 1.25 0 11-2.5 0 1.25 1.25 0 012.5 0z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="search-color-fg-muted">
              <svg height="16" class="octicon octicon-search color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M11.5 7a4.499 4.499 0 11-8.998 0A4.499 4.499 0 0111.5 7zm-.82 4.74a6 6 0 111.06-1.06l3.04 3.04a.75.75 0 11-1.06 1.06l-3.04-3.04z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="sun-color-fg-muted">
              <svg height="16" class="octicon octicon-sun color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M8 10.5a2.5 2.5 0 100-5 2.5 2.5 0 000 5zM8 12a4 4 0 100-8 4 4 0 000 8zM8 0a.75.75 0 01.75.75v1.5a.75.75 0 01-1.5 0V.75A.75.75 0 018 0zm0 13a.75.75 0 01.75.75v1.5a.75.75 0 01-1.5 0v-1.5A.75.75 0 018 13zM2.343 2.343a.75.75 0 011.061 0l1.06 1.061a.75.75 0 01-1.06 1.06l-1.06-1.06a.75.75 0 010-1.06zm9.193 9.193a.75.75 0 011.06 0l1.061 1.06a.75.75 0 01-1.06 1.061l-1.061-1.06a.75.75 0 010-1.061zM16 8a.75.75 0 01-.75.75h-1.5a.75.75 0 010-1.5h1.5A.75.75 0 0116 8zM3 8a.75.75 0 01-.75.75H.75a.75.75 0 010-1.5h1.5A.75.75 0 013 8zm10.657-5.657a.75.75 0 010 1.061l-1.061 1.06a.75.75 0 11-1.06-1.06l1.06-1.06a.75.75 0 011.06 0zm-9.193 9.193a.75.75 0 010 1.06l-1.06 1.061a.75.75 0 11-1.061-1.06l1.06-1.061a.75.75 0 011.061 0z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="sync-color-fg-muted">
              <svg height="16" class="octicon octicon-sync color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M8 2.5a5.487 5.487 0 00-4.131 1.869l1.204 1.204A.25.25 0 014.896 6H1.25A.25.25 0 011 5.75V2.104a.25.25 0 01.427-.177l1.38 1.38A7.001 7.001 0 0114.95 7.16a.75.75 0 11-1.49.178A5.501 5.501 0 008 2.5zM1.705 8.005a.75.75 0 01.834.656 5.501 5.501 0 009.592 2.97l-1.204-1.204a.25.25 0 01.177-.427h3.646a.25.25 0 01.25.25v3.646a.25.25 0 01-.427.177l-1.38-1.38A7.001 7.001 0 011.05 8.84a.75.75 0 01.656-.834z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="trash-color-fg-muted">
              <svg height="16" class="octicon octicon-trash color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M6.5 1.75a.25.25 0 01.25-.25h2.5a.25.25 0 01.25.25V3h-3V1.75zm4.5 0V3h2.25a.75.75 0 010 1.5H2.75a.75.75 0 010-1.5H5V1.75C5 .784 5.784 0 6.75 0h2.5C10.216 0 11 .784 11 1.75zM4.496 6.675a.75.75 0 10-1.492.15l.66 6.6A1.75 1.75 0 005.405 15h5.19c.9 0 1.652-.681 1.741-1.576l.66-6.6a.75.75 0 00-1.492-.149l-.66 6.6a.25.25 0 01-.249.225h-5.19a.25.25 0 01-.249-.225l-.66-6.6z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="key-color-fg-muted">
              <svg height="16" class="octicon octicon-key color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M6.5 5.5a4 4 0 112.731 3.795.75.75 0 00-.768.18L7.44 10.5H6.25a.75.75 0 00-.75.75v1.19l-.06.06H4.25a.75.75 0 00-.75.75v1.19l-.06.06H1.75a.25.25 0 01-.25-.25v-1.69l5.024-5.023a.75.75 0 00.181-.768A3.995 3.995 0 016.5 5.5zm4-5.5a5.5 5.5 0 00-5.348 6.788L.22 11.72a.75.75 0 00-.22.53v2C0 15.216.784 16 1.75 16h2a.75.75 0 00.53-.22l.5-.5a.75.75 0 00.22-.53V14h.75a.75.75 0 00.53-.22l.5-.5a.75.75 0 00.22-.53V12h.75a.75.75 0 00.53-.22l.932-.932A5.5 5.5 0 1010.5 0zm.5 6a1 1 0 100-2 1 1 0 000 2z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="comment-discussion-color-fg-muted">
              <svg height="16" class="octicon octicon-comment-discussion color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M1.5 2.75a.25.25 0 01.25-.25h8.5a.25.25 0 01.25.25v5.5a.25.25 0 01-.25.25h-3.5a.75.75 0 00-.53.22L3.5 11.44V9.25a.75.75 0 00-.75-.75h-1a.25.25 0 01-.25-.25v-5.5zM1.75 1A1.75 1.75 0 000 2.75v5.5C0 9.216.784 10 1.75 10H2v1.543a1.457 1.457 0 002.487 1.03L7.061 10h3.189A1.75 1.75 0 0012 8.25v-5.5A1.75 1.75 0 0010.25 1h-8.5zM14.5 4.75a.25.25 0 00-.25-.25h-.5a.75.75 0 110-1.5h.5c.966 0 1.75.784 1.75 1.75v5.5A1.75 1.75 0 0114.25 12H14v1.543a1.457 1.457 0 01-2.487 1.03L9.22 12.28a.75.75 0 111.06-1.06l2.22 2.22v-2.19a.75.75 0 01.75-.75h1a.25.25 0 00.25-.25v-5.5z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="bell-color-fg-muted">
              <svg height="16" class="octicon octicon-bell color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path d="M8 16a2 2 0 001.985-1.75c.017-.137-.097-.25-.235-.25h-3.5c-.138 0-.252.113-.235.25A2 2 0 008 16z"></path><path fill-rule="evenodd" d="M8 1.5A3.5 3.5 0 004.5 5v2.947c0 .346-.102.683-.294.97l-1.703 2.556a.018.018 0 00-.003.01l.001.006c0 .002.002.004.004.006a.017.017 0 00.006.004l.007.001h10.964l.007-.001a.016.016 0 00.006-.004.016.016 0 00.004-.006l.001-.007a.017.017 0 00-.003-.01l-1.703-2.554a1.75 1.75 0 01-.294-.97V5A3.5 3.5 0 008 1.5zM3 5a5 5 0 0110 0v2.947c0 .05.015.098.042.139l1.703 2.555A1.518 1.518 0 0113.482 13H2.518a1.518 1.518 0 01-1.263-2.36l1.703-2.554A.25.25 0 003 7.947V5z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="bell-slash-color-fg-muted">
              <svg height="16" class="octicon octicon-bell-slash color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M8 1.5c-.997 0-1.895.416-2.534 1.086A.75.75 0 014.38 1.55 5 5 0 0113 5v2.373a.75.75 0 01-1.5 0V5A3.5 3.5 0 008 1.5zM4.182 4.31L1.19 2.143a.75.75 0 10-.88 1.214L3 5.305v2.642a.25.25 0 01-.042.139L1.255 10.64A1.518 1.518 0 002.518 13h11.108l1.184.857a.75.75 0 10.88-1.214l-1.375-.996a1.196 1.196 0 00-.013-.01L4.198 4.321a.733.733 0 00-.016-.011zm7.373 7.19L4.5 6.391v1.556c0 .346-.102.683-.294.97l-1.703 2.556a.018.018 0 00-.003.01.015.015 0 00.005.012.017.017 0 00.006.004l.007.001h9.037zM8 16a2 2 0 001.985-1.75c.017-.137-.097-.25-.235-.25h-3.5c-.138 0-.252.113-.235.25A2 2 0 008 16z"></path></svg>
            </div>
            <div data-targets="command-palette-page-stack.localOcticons" data-octicon-id="paintbrush-color-fg-muted">
              <svg height="16" class="octicon octicon-paintbrush color-fg-muted" viewBox="0 0 16 16" version="1.1" width="16" aria-hidden="true"><path fill-rule="evenodd" d="M11.134 1.535C9.722 2.562 8.16 4.057 6.889 5.312 5.8 6.387 5.041 7.401 4.575 8.294a3.745 3.745 0 00-3.227 1.054c-.43.431-.69 1.066-.86 1.657a11.982 11.982 0 00-.358 1.914A21.263 21.263 0 000 15.203v.054l.75-.007-.007.75h.054a14.404 14.404 0 00.654-.012 21.243 21.243 0 001.63-.118c.62-.07 1.3-.18 1.914-.357.592-.17 1.226-.43 1.657-.861a3.745 3.745 0 001.055-3.217c.908-.461 1.942-1.216 3.04-2.3 1.279-1.262 2.764-2.825 3.775-4.249.501-.706.923-1.428 1.125-2.096.2-.659.235-1.469-.368-2.07-.606-.607-1.42-.55-2.069-.34-.66.213-1.376.646-2.076 1.155zm-3.95 8.48a3.76 3.76 0 00-1.19-1.192 9.758 9.758 0 011.161-1.607l1.658 1.658a9.853 9.853 0 01-1.63 1.142zM.742 16l.007-.75-.75.008A.75.75 0 00.743 16zM12.016 2.749c-1.224.89-2.605 2.189-3.822 3.384l1.718 1.718c1.21-1.205 2.51-2.597 3.387-3.833.47-.662.78-1.227.912-1.662.134-.444.032-.551.009-.575h-.001V1.78c-.014-.014-.112-.113-.548.027-.432.14-.995.462-1.655.942zM1.62 13.089a19.56 19.56 0 00-.104 1.395 19.55 19.55 0 001.396-.104 10.528 10.528 0 001.668-.309c.526-.151.856-.325 1.011-.48a2.25 2.25 0 00-3.182-3.182c-.155.155-.329.485-.48 1.01a10.515 10.515 0 00-.309 1.67z"></path></svg>
            </div>

            <command-palette-item-group
              data-group-id="top"
              data-group-title="Top result"
              data-group-hint=""
              data-group-limits="{}"
              data-default-priority="0"
            >
            </command-palette-item-group>
            <command-palette-item-group
              data-group-id="commands"
              data-group-title="Commands"
              data-group-hint="Type &gt; to filter"
              data-group-limits="{&quot;static_items_page&quot;:50,&quot;issue&quot;:50,&quot;pull_request&quot;:50,&quot;discussion&quot;:50}"
              data-default-priority="1"
            >
            </command-palette-item-group>
            <command-palette-item-group
              data-group-id="global_commands"
              data-group-title="Global Commands"
              data-group-hint="Type &gt; to filter"
              data-group-limits="{&quot;issue&quot;:0,&quot;pull_request&quot;:0,&quot;discussion&quot;:0}"
              data-default-priority="2"
            >
            </command-palette-item-group>
            <command-palette-item-group
              data-group-id="this_page"
              data-group-title="This Page"
              data-group-hint=""
              data-group-limits="{}"
              data-default-priority="3"
            >
            </command-palette-item-group>
            <command-palette-item-group
              data-group-id="files"
              data-group-title="Files"
              data-group-hint=""
              data-group-limits="{}"
              data-default-priority="4"
            >
            </command-palette-item-group>
            <command-palette-item-group
              data-group-id="default"
              data-group-title="Default"
              data-group-hint=""
              data-group-limits="{&quot;static_items_page&quot;:50}"
              data-default-priority="5"
            >
            </command-palette-item-group>
            <command-palette-item-group
              data-group-id="pages"
              data-group-title="Pages"
              data-group-hint=""
              data-group-limits="{&quot;repository&quot;:10}"
              data-default-priority="6"
            >
            </command-palette-item-group>
            <command-palette-item-group
              data-group-id="access_policies"
              data-group-title="Access Policies"
              data-group-hint=""
              data-group-limits="{}"
              data-default-priority="7"
            >
            </command-palette-item-group>
            <command-palette-item-group
              data-group-id="organizations"
              data-group-title="Organizations"
              data-group-hint=""
              data-group-limits="{}"
              data-default-priority="8"
            >
            </command-palette-item-group>
            <command-palette-item-group
              data-group-id="repositories"
              data-group-title="Repositories"
              data-group-hint=""
              data-group-limits="{}"
              data-default-priority="9"
            >
            </command-palette-item-group>
            <command-palette-item-group
              data-group-id="references"
              data-group-title="Issues, pull requests, and discussions"
              data-group-hint="Type # to filter"
              data-group-limits="{}"
              data-default-priority="10"
            >
            </command-palette-item-group>
            <command-palette-item-group
              data-group-id="teams"
              data-group-title="Teams"
              data-group-hint=""
              data-group-limits="{}"
              data-default-priority="11"
            >
            </command-palette-item-group>
            <command-palette-item-group
              data-group-id="users"
              data-group-title="Users"
              data-group-hint=""
              data-group-limits="{}"
              data-default-priority="12"
            >
            </command-palette-item-group>
            <command-palette-item-group
              data-group-id="projects"
              data-group-title="Projects"
              data-group-hint=""
              data-group-limits="{}"
              data-default-priority="13"
            >
            </command-palette-item-group>
            <command-palette-item-group
              data-group-id="footer"
              data-group-title="Footer"
              data-group-hint=""
              data-group-limits="{}"
              data-default-priority="14"
            >
            </command-palette-item-group>
            <command-palette-item-group
              data-group-id="modes_help"
              data-group-title="Modes"
              data-group-hint=""
              data-group-limits="{}"
              data-default-priority="15"
            >
            </command-palette-item-group>
            <command-palette-item-group
              data-group-id="filters_help"
              data-group-title="Use filters in issues, pull requests, discussions, and projects"
              data-group-hint=""
              data-group-limits="{}"
              data-default-priority="16"
            >
            </command-palette-item-group>

            <command-palette-page
              data-page-title="sean207cc"
              data-scope-id="U_kgDOBs3vmA"
              data-scope-type="owner"
              data-targets="command-palette-page-stack.defaultPages"
              hidden
            >
            </command-palette-page>
            <command-palette-page
              data-page-title="AI-course"
              data-scope-id="R_kgDOIlI2oQ"
              data-scope-type="repository"
              data-targets="command-palette-page-stack.defaultPages"
              hidden
            >
            </command-palette-page>
        </div>

        <command-palette-page data-is-root>
        </command-palette-page>
          <command-palette-page
            data-page-title="sean207cc"
            data-scope-id="U_kgDOBs3vmA"
            data-scope-type="owner"
          >
          </command-palette-page>
          <command-palette-page
            data-page-title="AI-course"
            data-scope-id="R_kgDOIlI2oQ"
            data-scope-type="repository"
          >
          </command-palette-page>
      </command-palette-page-stack>

      <server-defined-provider data-type="search-links" data-targets="command-palette.serverDefinedProviderElements"></server-defined-provider>
      <server-defined-provider data-type="help" data-targets="command-palette.serverDefinedProviderElements">
          <command-palette-help
            data-group="modes_help"
              data-prefix="#"
              data-scope-types="[&quot;&quot;]"
          >
            <span data-target="command-palette-help.titleElement">Search for <strong>issues</strong> and <strong>pull requests</strong></span>
              <span data-target="command-palette-help.hintElement">
                <kbd class="hx_kbd">#</kbd>
              </span>
          </command-palette-help>
          <command-palette-help
            data-group="modes_help"
              data-prefix="#"
              data-scope-types="[&quot;owner&quot;,&quot;repository&quot;]"
          >
            <span data-target="command-palette-help.titleElement">Search for <strong>issues, pull requests, discussions,</strong> and <strong>projects</strong></span>
              <span data-target="command-palette-help.hintElement">
                <kbd class="hx_kbd">#</kbd>
              </span>
          </command-palette-help>
          <command-palette-help
            data-group="modes_help"
              data-prefix="@"
              data-scope-types="[&quot;&quot;]"
          >
            <span data-target="command-palette-help.titleElement">Search for <strong>organizations, repositories,</strong> and <strong>users</strong></span>
              <span data-target="command-palette-help.hintElement">
                <kbd class="hx_kbd">@</kbd>
              </span>
          </command-palette-help>
          <command-palette-help
            data-group="modes_help"
              data-prefix="!"
              data-scope-types="[&quot;owner&quot;,&quot;repository&quot;]"
          >
            <span data-target="command-palette-help.titleElement">Search for <strong>projects</strong></span>
              <span data-target="command-palette-help.hintElement">
                <kbd class="hx_kbd">!</kbd>
              </span>
          </command-palette-help>
          <command-palette-help
            data-group="modes_help"
              data-prefix="/"
              data-scope-types="[&quot;repository&quot;]"
          >
            <span data-target="command-palette-help.titleElement">Search for <strong>files</strong></span>
              <span data-target="command-palette-help.hintElement">
                <kbd class="hx_kbd">/</kbd>
              </span>
          </command-palette-help>
          <command-palette-help
            data-group="modes_help"
              data-prefix="&gt;"
          >
            <span data-target="command-palette-help.titleElement">Activate <strong>command mode</strong></span>
              <span data-target="command-palette-help.hintElement">
                <kbd class="hx_kbd">&gt;</kbd>
              </span>
          </command-palette-help>
          <command-palette-help
            data-group="filters_help"
              data-prefix="# author:@me"
          >
            <span data-target="command-palette-help.titleElement">Search your issues, pull requests, and discussions</span>
              <span data-target="command-palette-help.hintElement">
                <kbd class="hx_kbd"># author:@me</kbd>
              </span>
          </command-palette-help>
          <command-palette-help
            data-group="filters_help"
              data-prefix="# author:@me"
          >
            <span data-target="command-palette-help.titleElement">Search your issues, pull requests, and discussions</span>
              <span data-target="command-palette-help.hintElement">
                <kbd class="hx_kbd"># author:@me</kbd>
              </span>
          </command-palette-help>
          <command-palette-help
            data-group="filters_help"
              data-prefix="# is:pr"
          >
            <span data-target="command-palette-help.titleElement">Filter to pull requests</span>
              <span data-target="command-palette-help.hintElement">
                <kbd class="hx_kbd"># is:pr</kbd>
              </span>
          </command-palette-help>
          <command-palette-help
            data-group="filters_help"
              data-prefix="# is:issue"
          >
            <span data-target="command-palette-help.titleElement">Filter to issues</span>
              <span data-target="command-palette-help.hintElement">
                <kbd class="hx_kbd"># is:issue</kbd>
              </span>
          </command-palette-help>
          <command-palette-help
            data-group="filters_help"
              data-prefix="# is:discussion"
              data-scope-types="[&quot;owner&quot;,&quot;repository&quot;]"
          >
            <span data-target="command-palette-help.titleElement">Filter to discussions</span>
              <span data-target="command-palette-help.hintElement">
                <kbd class="hx_kbd"># is:discussion</kbd>
              </span>
          </command-palette-help>
          <command-palette-help
            data-group="filters_help"
              data-prefix="# is:project"
              data-scope-types="[&quot;owner&quot;,&quot;repository&quot;]"
          >
            <span data-target="command-palette-help.titleElement">Filter to projects</span>
              <span data-target="command-palette-help.hintElement">
                <kbd class="hx_kbd"># is:project</kbd>
              </span>
          </command-palette-help>
          <command-palette-help
            data-group="filters_help"
              data-prefix="# is:open"
          >
            <span data-target="command-palette-help.titleElement">Filter to open issues, pull requests, and discussions</span>
              <span data-target="command-palette-help.hintElement">
                <kbd class="hx_kbd"># is:open</kbd>
              </span>
          </command-palette-help>
      </server-defined-provider>

        <server-defined-provider
          data-type="commands"
          data-fetch-debounce="0"
            data-src="/command_palette/commands"
          data-supported-modes="[]"
            data-supports-commands
          
          data-targets="command-palette.serverDefinedProviderElements"
          ></server-defined-provider>
        <server-defined-provider
          data-type="prefetched"
          data-fetch-debounce="0"
            data-src="/command_palette/jump_to_page_navigation"
          data-supported-modes="[&quot;&quot;]"
            data-supported-scope-types="[&quot;&quot;,&quot;owner&quot;,&quot;repository&quot;]"
          
          data-targets="command-palette.serverDefinedProviderElements"
          ></server-defined-provider>
        <server-defined-provider
          data-type="remote"
          data-fetch-debounce="200"
            data-src="/command_palette/issues"
          data-supported-modes="[&quot;#&quot;,&quot;#&quot;]"
            data-supported-scope-types="[&quot;owner&quot;,&quot;repository&quot;,&quot;&quot;]"
          
          data-targets="command-palette.serverDefinedProviderElements"
          ></server-defined-provider>
        <server-defined-provider
          data-type="remote"
          data-fetch-debounce="200"
            data-src="/command_palette/jump_to"
          data-supported-modes="[&quot;@&quot;,&quot;@&quot;]"
            data-supported-scope-types="[&quot;&quot;,&quot;owner&quot;]"
          
          data-targets="command-palette.serverDefinedProviderElements"
          ></server-defined-provider>
        <server-defined-provider
          data-type="remote"
          data-fetch-debounce="200"
            data-src="/command_palette/jump_to_members_only"
          data-supported-modes="[&quot;@&quot;,&quot;@&quot;,&quot;&quot;,&quot;&quot;]"
            data-supported-scope-types="[&quot;&quot;,&quot;owner&quot;]"
          
          data-targets="command-palette.serverDefinedProviderElements"
          ></server-defined-provider>
        <server-defined-provider
          data-type="prefetched"
          data-fetch-debounce="0"
            data-src="/command_palette/jump_to_members_only_prefetched"
          data-supported-modes="[&quot;@&quot;,&quot;@&quot;,&quot;&quot;,&quot;&quot;]"
            data-supported-scope-types="[&quot;&quot;,&quot;owner&quot;]"
          
          data-targets="command-palette.serverDefinedProviderElements"
          ></server-defined-provider>
        <server-defined-provider
          data-type="files"
          data-fetch-debounce="0"
            data-src="/command_palette/files"
          data-supported-modes="[&quot;/&quot;]"
            data-supported-scope-types="[&quot;repository&quot;]"
          
          data-targets="command-palette.serverDefinedProviderElements"
          ></server-defined-provider>
        <server-defined-provider
          data-type="remote"
          data-fetch-debounce="200"
            data-src="/command_palette/discussions"
          data-supported-modes="[&quot;#&quot;]"
            data-supported-scope-types="[&quot;owner&quot;,&quot;repository&quot;]"
          
          data-targets="command-palette.serverDefinedProviderElements"
          ></server-defined-provider>
        <server-defined-provider
          data-type="remote"
          data-fetch-debounce="200"
            data-src="/command_palette/projects"
          data-supported-modes="[&quot;#&quot;,&quot;!&quot;]"
            data-supported-scope-types="[&quot;owner&quot;,&quot;repository&quot;]"
          
          data-targets="command-palette.serverDefinedProviderElements"
          ></server-defined-provider>
        <server-defined-provider
          data-type="prefetched"
          data-fetch-debounce="0"
            data-src="/command_palette/recent_issues"
          data-supported-modes="[&quot;#&quot;,&quot;#&quot;]"
            data-supported-scope-types="[&quot;owner&quot;,&quot;repository&quot;,&quot;&quot;]"
          
          data-targets="command-palette.serverDefinedProviderElements"
          ></server-defined-provider>
        <server-defined-provider
          data-type="remote"
          data-fetch-debounce="200"
            data-src="/command_palette/teams"
          data-supported-modes="[&quot;@&quot;,&quot;&quot;]"
            data-supported-scope-types="[&quot;owner&quot;]"
          
          data-targets="command-palette.serverDefinedProviderElements"
          ></server-defined-provider>
        <server-defined-provider
          data-type="remote"
          data-fetch-debounce="200"
            data-src="/command_palette/name_with_owner_repository"
          data-supported-modes="[&quot;@&quot;,&quot;@&quot;,&quot;&quot;,&quot;&quot;]"
            data-supported-scope-types="[&quot;&quot;,&quot;owner&quot;]"
          
          data-targets="command-palette.serverDefinedProviderElements"
          ></server-defined-provider>
    </command-palette>
  </details-dialog>
</details>

<div class="position-fixed bottom-0 left-0 ml-5 mb-5 js-command-palette-toasts" style="z-index: 1000">
  <div hidden class="Toast Toast--loading">
    <span class="Toast-icon">
      <svg class="Toast--spinner" viewBox="0 0 32 32" width="18" height="18" aria-hidden="true">
        <path
          fill="#959da5"
          d="M16 0 A16 16 0 0 0 16 32 A16 16 0 0 0 16 0 M16 4 A12 12 0 0 1 16 28 A12 12 0 0 1 16 4"
        />
        <path fill="#ffffff" d="M16 0 A16 16 0 0 1 32 16 L28 16 A12 12 0 0 0 16 4z"></path>
      </svg>
    </span>
    <span class="Toast-content"></span>
  </div>

  <div hidden class="anim-fade-in fast Toast Toast--error">
    <span class="Toast-icon">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-stop">
    <path fill-rule="evenodd" d="M4.47.22A.75.75 0 015 0h6a.75.75 0 01.53.22l4.25 4.25c.141.14.22.331.22.53v6a.75.75 0 01-.22.53l-4.25 4.25A.75.75 0 0111 16H5a.75.75 0 01-.53-.22L.22 11.53A.75.75 0 010 11V5a.75.75 0 01.22-.53L4.47.22zm.84 1.28L1.5 5.31v5.38l3.81 3.81h5.38l3.81-3.81V5.31L10.69 1.5H5.31zM8 4a.75.75 0 01.75.75v3.5a.75.75 0 01-1.5 0v-3.5A.75.75 0 018 4zm0 8a1 1 0 100-2 1 1 0 000 2z"></path>
</svg>
    </span>
    <span class="Toast-content"></span>
  </div>

  <div hidden class="anim-fade-in fast Toast Toast--warning">
    <span class="Toast-icon">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-alert">
    <path fill-rule="evenodd" d="M8.22 1.754a.25.25 0 00-.44 0L1.698 13.132a.25.25 0 00.22.368h12.164a.25.25 0 00.22-.368L8.22 1.754zm-1.763-.707c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0114.082 15H1.918a1.75 1.75 0 01-1.543-2.575L6.457 1.047zM9 11a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.25a.75.75 0 00-1.5 0v2.5a.75.75 0 001.5 0v-2.5z"></path>
</svg>
    </span>
    <span class="Toast-content"></span>
  </div>


  <div hidden class="anim-fade-in fast Toast Toast--success">
    <span class="Toast-icon">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
    </span>
    <span class="Toast-content"></span>
  </div>

  <div hidden class="anim-fade-in fast Toast">
    <span class="Toast-icon">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-info">
    <path fill-rule="evenodd" d="M8 1.5a6.5 6.5 0 100 13 6.5 6.5 0 000-13zM0 8a8 8 0 1116 0A8 8 0 010 8zm6.5-.25A.75.75 0 017.25 7h1a.75.75 0 01.75.75v2.75h.25a.75.75 0 010 1.5h-2a.75.75 0 010-1.5h.25v-2h-.25a.75.75 0 01-.75-.75zM8 6a1 1 0 100-2 1 1 0 000 2z"></path>
</svg>
    </span>
    <span class="Toast-content"></span>
  </div>
</div>


  <div
    class="application-main "
    data-commit-hovercards-enabled
    data-discussion-hovercards-enabled
    data-issue-and-pr-hovercards-enabled
  >
        <div itemscope itemtype="http://schema.org/SoftwareSourceCode" class="">
    <main id="js-repo-pjax-container" >
      
  


    





  
  <div id="repository-container-header"  class="pt-3 hide-full-screen" style="background-color: var(--color-page-header-bg);" data-turbo-replace>

      <div class="d-flex flex-wrap flex-justify-end mb-3  px-3 px-md-4 px-lg-5" style="gap: 1rem;">

        <div class="flex-auto min-width-0 width-fit mr-3">
            
  <div class=" d-flex flex-wrap flex-items-center wb-break-word f3 text-normal">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-repo-forked color-fg-muted mr-2">
    <path fill-rule="evenodd" d="M5 3.25a.75.75 0 11-1.5 0 .75.75 0 011.5 0zm0 2.122a2.25 2.25 0 10-1.5 0v.878A2.25 2.25 0 005.75 8.5h1.5v2.128a2.251 2.251 0 101.5 0V8.5h1.5a2.25 2.25 0 002.25-2.25v-.878a2.25 2.25 0 10-1.5 0v.878a.75.75 0 01-.75.75h-4.5A.75.75 0 015 6.25v-.878zm3.75 7.378a.75.75 0 11-1.5 0 .75.75 0 011.5 0zm3-8.75a.75.75 0 100-1.5.75.75 0 000 1.5z"></path>
</svg>
    
    <span class="author flex-self-stretch" itemprop="author">
      <a class="url fn" rel="author" data-hovercard-type="user" data-hovercard-url="/users/sean207cc/hovercard" data-octo-click="hovercard-link-click" data-octo-dimensions="link_type:self" href="/sean207cc">sean207cc</a>
    </span>
    <span class="mx-1 flex-self-stretch color-fg-muted">/</span>
    <strong itemprop="name" class="mr-2 flex-self-stretch">
      <a data-pjax="#repo-content-pjax-container" data-turbo-frame="repo-content-turbo-frame" href="/sean207cc/AI-course">AI-course</a>
    </strong>

    <span></span><span class="Label Label--secondary v-align-middle mr-1">Public</span>
  </div>
    <span class="text-small lh-condensed-ultra no-wrap mt-1" data-repository-hovercards-enabled>
      forked from <a data-hovercard-type="repository" data-hovercard-url="/rkuo2000/AI-course/hovercard" href="/rkuo2000/AI-course">rkuo2000/AI-course</a>
    </span>


        </div>

          <ul class="pagehead-actions flex-shrink-0 d-none d-md-inline" style="padding: 2px 0;">

      <li>
  <div class="float-left" data-test-selector="pin-repo-button">
    <form data-turbo="false" action="/sean207cc/AI-course/profile_pin" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="Fd3bIgo83olSV4eWZ1OimKyVjELaE3pK4DZNza9AQbxXmpvCb4Zjs3ppD92J6o-g-mW5mhnQNBot5nsDxp13SA" autocomplete="off" />
        <button title="Pin this repository to your profile" type="submit" data-view-component="true" class="btn-sm btn">    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-pin mr-2">
    <path fill-rule="evenodd" d="M4.456.734a1.75 1.75 0 012.826.504l.613 1.327a3.081 3.081 0 002.084 1.707l2.454.584c1.332.317 1.8 1.972.832 2.94L11.06 10l3.72 3.72a.75.75 0 11-1.061 1.06L10 11.06l-2.204 2.205c-.968.968-2.623.5-2.94-.832l-.584-2.454a3.081 3.081 0 00-1.707-2.084l-1.327-.613a1.75 1.75 0 01-.504-2.826L4.456.734zM5.92 1.866a.25.25 0 00-.404-.072L1.794 5.516a.25.25 0 00.072.404l1.328.613A4.582 4.582 0 015.73 9.63l.584 2.454a.25.25 0 00.42.12l5.47-5.47a.25.25 0 00-.12-.42L9.63 5.73a4.581 4.581 0 01-3.098-2.537L5.92 1.866z"></path>
</svg>Pin
</button></form>  </div>
</li>


  <li>
          <notifications-list-subscription-form
      data-action="notifications-dialog-label-toggled:notifications-list-subscription-form#handleDialogLabelToggle"
      class="f5 position-relative"
    >
      <details
        class="details-reset details-overlay f5 position-relative"
        data-target="notifications-list-subscription-form.details"
        data-action="toggle:notifications-list-subscription-form#detailsToggled"
      >

        <summary data-hydro-click="{&quot;event_type&quot;:&quot;repository.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;WATCH_BUTTON&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="11b82138e50f2ea69be92b33b91fa9e2d0fea3a0fd92236b0c70f55751fa0355" data-ga-click="Repository, click Watch settings, action:blob#show" aria-label="Notification settings" data-view-component="true" class="btn-sm btn">    <span data-menu-button>
            <span
              hidden
              
              data-target="notifications-list-subscription-form.unwatchButtonCopy"
            >
              <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-eye">
    <path fill-rule="evenodd" d="M1.679 7.932c.412-.621 1.242-1.75 2.366-2.717C5.175 4.242 6.527 3.5 8 3.5c1.473 0 2.824.742 3.955 1.715 1.124.967 1.954 2.096 2.366 2.717a.119.119 0 010 .136c-.412.621-1.242 1.75-2.366 2.717C10.825 11.758 9.473 12.5 8 12.5c-1.473 0-2.824-.742-3.955-1.715C2.92 9.818 2.09 8.69 1.679 8.068a.119.119 0 010-.136zM8 2c-1.981 0-3.67.992-4.933 2.078C1.797 5.169.88 6.423.43 7.1a1.619 1.619 0 000 1.798c.45.678 1.367 1.932 2.637 3.024C4.329 13.008 6.019 14 8 14c1.981 0 3.67-.992 4.933-2.078 1.27-1.091 2.187-2.345 2.637-3.023a1.619 1.619 0 000-1.798c-.45-.678-1.367-1.932-2.637-3.023C11.671 2.992 9.981 2 8 2zm0 8a2 2 0 100-4 2 2 0 000 4z"></path>
</svg>
              Unwatch
            </span>
            <span
              hidden
              
              data-target="notifications-list-subscription-form.stopIgnoringButtonCopy"
            >
              <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-bell-slash">
    <path fill-rule="evenodd" d="M8 1.5c-.997 0-1.895.416-2.534 1.086A.75.75 0 014.38 1.55 5 5 0 0113 5v2.373a.75.75 0 01-1.5 0V5A3.5 3.5 0 008 1.5zM4.182 4.31L1.19 2.143a.75.75 0 10-.88 1.214L3 5.305v2.642a.25.25 0 01-.042.139L1.255 10.64A1.518 1.518 0 002.518 13h11.108l1.184.857a.75.75 0 10.88-1.214l-1.375-.996a1.196 1.196 0 00-.013-.01L4.198 4.321a.733.733 0 00-.016-.011zm7.373 7.19L4.5 6.391v1.556c0 .346-.102.683-.294.97l-1.703 2.556a.018.018 0 00-.003.01.015.015 0 00.005.012.017.017 0 00.006.004l.007.001h9.037zM8 16a2 2 0 001.985-1.75c.017-.137-.097-.25-.235-.25h-3.5c-.138 0-.252.113-.235.25A2 2 0 008 16z"></path>
</svg>
              Stop ignoring
            </span>
            <span
              
              
              data-target="notifications-list-subscription-form.watchButtonCopy"
            >
              <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-eye">
    <path fill-rule="evenodd" d="M1.679 7.932c.412-.621 1.242-1.75 2.366-2.717C5.175 4.242 6.527 3.5 8 3.5c1.473 0 2.824.742 3.955 1.715 1.124.967 1.954 2.096 2.366 2.717a.119.119 0 010 .136c-.412.621-1.242 1.75-2.366 2.717C10.825 11.758 9.473 12.5 8 12.5c-1.473 0-2.824-.742-3.955-1.715C2.92 9.818 2.09 8.69 1.679 8.068a.119.119 0 010-.136zM8 2c-1.981 0-3.67.992-4.933 2.078C1.797 5.169.88 6.423.43 7.1a1.619 1.619 0 000 1.798c.45.678 1.367 1.932 2.637 3.024C4.329 13.008 6.019 14 8 14c1.981 0 3.67-.992 4.933-2.078 1.27-1.091 2.187-2.345 2.637-3.023a1.619 1.619 0 000-1.798c-.45-.678-1.367-1.932-2.637-3.023C11.671 2.992 9.981 2 8 2zm0 8a2 2 0 100-4 2 2 0 000 4z"></path>
</svg>
              Watch
            </span>
          </span>
            <span id="repo-notifications-counter" data-target="notifications-list-subscription-form.socialCount" data-pjax-replace="true" data-turbo-replace="true" title="0" data-view-component="true" class="Counter">0</span>
          <span class="dropdown-caret"></span>
</summary>
        <details-menu
          class="SelectMenu  "
          role="menu"
          data-target="notifications-list-subscription-form.menu"
          
        >
          <div class="SelectMenu-modal notifications-component-menu-modal">
            <header class="SelectMenu-header">
              <h3 class="SelectMenu-title">Notifications</h3>
              <button class="SelectMenu-closeButton" type="button" aria-label="Close menu" data-action="click:notifications-list-subscription-form#closeMenu">
                <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path>
</svg>
              </button>
            </header>

            <div class="SelectMenu-list">
              <form data-target="notifications-list-subscription-form.form" data-action="submit:notifications-list-subscription-form#submitForm" data-turbo="false" action="/notifications/subscribe" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="Xr-uOuYwhbXkSv8gCi9jBsG0pjgGF8Am7DQfqgz3B_8Ki95fx1j-DKx_Xrrgrq4h-KePaUC5HoiPgqRpqqjdRg" autocomplete="off" />

                <input type="hidden" name="repository_id" value="575813281">

                <button
                  type="submit"
                  name="do"
                  value="included"
                  class="SelectMenu-item flex-items-start"
                  role="menuitemradio"
                  aria-checked="true"
                  data-targets="notifications-list-subscription-form.subscriptionButtons"
                  
                >
                  <span class="f5">
                    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check SelectMenu-icon SelectMenu-icon--check">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
                  </span>
                  <div>
                    <div class="f5 text-bold">
                      Participating and @mentions
                    </div>
                    <div class="text-small color-fg-muted text-normal pb-1">
                      Only receive notifications from this repository when participating or @mentioned.
                    </div>
                  </div>
                </button>

                <button
                  type="submit"
                  name="do"
                  value="subscribed"
                  class="SelectMenu-item flex-items-start"
                  role="menuitemradio"
                  aria-checked="false"
                  data-targets="notifications-list-subscription-form.subscriptionButtons"
                >
                  <span class="f5">
                    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check SelectMenu-icon SelectMenu-icon--check">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
                  </span>
                  <div>
                    <div class="f5 text-bold">
                      All Activity
                    </div>
                    <div class="text-small color-fg-muted text-normal pb-1">
                      Notified of all notifications on this repository.
                    </div>
                  </div>
                </button>

                <button
                  type="submit"
                  name="do"
                  value="ignore"
                  class="SelectMenu-item flex-items-start"
                  role="menuitemradio"
                  aria-checked="false"
                  data-targets="notifications-list-subscription-form.subscriptionButtons"
                >
                  <span class="f5">
                    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check SelectMenu-icon SelectMenu-icon--check">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
                  </span>
                  <div>
                    <div class="f5 text-bold">
                      Ignore
                    </div>
                    <div class="text-small color-fg-muted text-normal pb-1">
                      Never be notified.
                    </div>
                  </div>
                </button>
</form>
              <button
                class="SelectMenu-item flex-items-start pr-3"
                type="button"
                role="menuitemradio"
                data-target="notifications-list-subscription-form.customButton"
                data-action="click:notifications-list-subscription-form#openCustomDialog"
                aria-haspopup="true"
                aria-checked="false"
                
              >
                <span class="f5">
                  <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check SelectMenu-icon SelectMenu-icon--check">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
                </span>
                <div>
                  <div class="d-flex flex-items-start flex-justify-between">
                    <div class="f5 text-bold">Custom</div>
                    <div class="f5 pr-1">
                      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-arrow-right">
    <path fill-rule="evenodd" d="M8.22 2.97a.75.75 0 011.06 0l4.25 4.25a.75.75 0 010 1.06l-4.25 4.25a.75.75 0 01-1.06-1.06l2.97-2.97H3.75a.75.75 0 010-1.5h7.44L8.22 4.03a.75.75 0 010-1.06z"></path>
</svg>
                    </div>
                  </div>
                  <div class="text-small color-fg-muted text-normal pb-1">
                    Select events you want to be notified of in addition to participating and @mentions.
                  </div>
                </div>
              </button>

                <div class="px-3 py-2 d-flex color-bg-subtle flex-items-center">
                  <span class="f5">
                    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-device-mobile SelectMenu-icon SelectMenu-icon--device-mobile">
    <path fill-rule="evenodd" d="M3.75 0A1.75 1.75 0 002 1.75v12.5c0 .966.784 1.75 1.75 1.75h8.5A1.75 1.75 0 0014 14.25V1.75A1.75 1.75 0 0012.25 0h-8.5zM3.5 1.75a.25.25 0 01.25-.25h8.5a.25.25 0 01.25.25v12.5a.25.25 0 01-.25.25h-8.5a.25.25 0 01-.25-.25V1.75zM8 13a1 1 0 100-2 1 1 0 000 2z"></path>
</svg>
                  </span>
                  <span className="text-small color-fg-muted text-normal pb-1">
                    Get push notifications on <a target="_blank" rel="noopener noreferrer" href="https://apps.apple.com/app/apple-store/id1477376905?ct=watch-dropdown&amp;mt=8&amp;pt=524675">iOS</a> or <a target="_blank" rel="noopener noreferrer" href="https://play.google.com/store/apps/details?id=com.github.android&amp;referrer=utm_campaign%3Dwatch-dropdown%26utm_medium%3Dweb%26utm_source%3Dgithub">Android</a>.
                  </span>
                </div>
            </div>
          </div>
        </details-menu>

        <details-dialog
          class="notifications-component-dialog "
          data-target="notifications-list-subscription-form.customDialog"
          aria-label="Custom dialog"
          hidden
        >
          <div class="SelectMenu-modal notifications-component-dialog-modal overflow-visible">
            <form data-target="notifications-list-subscription-form.customform" data-action="submit:notifications-list-subscription-form#submitCustomForm" data-turbo="false" action="/notifications/subscribe" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="Q1dYNNaZdi2Smv-APChqGTGcjZXP9K-0L9ft1KsH5I8XYyhR9_ENlNqvXhrWqac-CI-kxIlacRpMYVYXDVg-Ng" autocomplete="off" />

              <input type="hidden" name="repository_id" value="575813281">

              <header class="d-sm-none SelectMenu-header pb-0 border-bottom-0 px-2 px-sm-3">
                <h1 class="f3 SelectMenu-title d-inline-flex">
                  <button
                    class="color-bg-default border-0 px-2 py-0 m-0 Link--secondary f5"
                    aria-label="Return to menu"
                    type="button"
                    data-action="click:notifications-list-subscription-form#closeCustomDialog"
                  >
                    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-arrow-left">
    <path fill-rule="evenodd" d="M7.78 12.53a.75.75 0 01-1.06 0L2.47 8.28a.75.75 0 010-1.06l4.25-4.25a.75.75 0 011.06 1.06L4.81 7h7.44a.75.75 0 010 1.5H4.81l2.97 2.97a.75.75 0 010 1.06z"></path>
</svg>
                  </button>
                  Custom
                </h1>
              </header>

              <header class="d-none d-sm-flex flex-items-start pt-1">
                <button
                  class="border-0 px-2 pt-1 m-0 Link--secondary f5"
                  style="background-color: transparent;"
                  aria-label="Return to menu"
                  type="button"
                  data-action="click:notifications-list-subscription-form#closeCustomDialog"
                >
                  <svg style="position: relative; left: 2px; top: 1px" aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-arrow-left">
    <path fill-rule="evenodd" d="M7.78 12.53a.75.75 0 01-1.06 0L2.47 8.28a.75.75 0 010-1.06l4.25-4.25a.75.75 0 011.06 1.06L4.81 7h7.44a.75.75 0 010 1.5H4.81l2.97 2.97a.75.75 0 010 1.06z"></path>
</svg>
                </button>

                <h1 class="pt-1 pr-4 pb-0 pl-0 f5 text-bold">
                  Custom
                </h1>
              </header>

              <fieldset>
                <legend>
                  <div class="text-small color-fg-muted pt-0 pr-3 pb-3 pl-6 pl-sm-5 border-bottom mb-3">
                    Select events you want to be notified of in addition to participating and @mentions.
                  </div>
                </legend>
                <div data-target="notifications-list-subscription-form.labelInputs">
                </div>
                  <div class="form-checkbox mr-3 ml-6 ml-sm-5 mb-2 mt-0">
                    <label class="f5 text-normal">
                      <input
                        type="checkbox"
                        name="thread_types[]"
                        value="Issue"
                        data-targets="notifications-list-subscription-form.threadTypeCheckboxes"
                        data-action="change:notifications-list-subscription-form#threadTypeCheckboxesUpdated"
                        
                          aria-describedby="Issue-disabled"
                          aria-disabled="true"
                      >
                      Issues
                    </label>

                      <div
                        id="Issue-disabled"
                        class="color-fg-muted"
                        >
                        Issues are not enabled for this repository
                      </div>

                  </div>
                  <div class="form-checkbox mr-3 ml-6 ml-sm-5 mb-2 mt-0">
                    <label class="f5 text-normal">
                      <input
                        type="checkbox"
                        name="thread_types[]"
                        value="PullRequest"
                        data-targets="notifications-list-subscription-form.threadTypeCheckboxes"
                        data-action="change:notifications-list-subscription-form#threadTypeCheckboxesUpdated"
                        
                      >
                      Pull requests
                    </label>


                  </div>
                  <div class="form-checkbox mr-3 ml-6 ml-sm-5 mb-2 mt-0">
                    <label class="f5 text-normal">
                      <input
                        type="checkbox"
                        name="thread_types[]"
                        value="Release"
                        data-targets="notifications-list-subscription-form.threadTypeCheckboxes"
                        data-action="change:notifications-list-subscription-form#threadTypeCheckboxesUpdated"
                        
                      >
                      Releases
                    </label>


                  </div>
                  <div class="form-checkbox mr-3 ml-6 ml-sm-5 mb-2 mt-0">
                    <label class="f5 text-normal">
                      <input
                        type="checkbox"
                        name="thread_types[]"
                        value="Discussion"
                        data-targets="notifications-list-subscription-form.threadTypeCheckboxes"
                        data-action="change:notifications-list-subscription-form#threadTypeCheckboxesUpdated"
                        
                          aria-describedby="Discussion-disabled"
                          aria-disabled="true"
                      >
                      Discussions
                    </label>

                      <div
                        id="Discussion-disabled"
                        class="color-fg-muted"
                        >
                        Discussions are not enabled for this repository
                      </div>

                  </div>
                  <div class="form-checkbox mr-3 ml-6 ml-sm-5 mb-2 mt-0">
                    <label class="f5 text-normal">
                      <input
                        type="checkbox"
                        name="thread_types[]"
                        value="SecurityAlert"
                        data-targets="notifications-list-subscription-form.threadTypeCheckboxes"
                        data-action="change:notifications-list-subscription-form#threadTypeCheckboxesUpdated"
                        
                      >
                      Security alerts
                    </label>


                  </div>
              </fieldset>
              <div class="pt-2 pb-3 px-3 d-flex flex-justify-start flex-row-reverse">
                  <button name="do" value="custom" data-target="notifications-list-subscription-form.customSubmit" disabled="disabled" type="submit" data-view-component="true" class="btn-primary btn-sm btn ml-2">    Apply
</button>

                  <button data-action="click:notifications-list-subscription-form#resetForm" data-close-dialog="" type="button" data-view-component="true" class="btn-sm btn">    Cancel
</button>
              </div>
</form>          </div>
        </details-dialog>


        <div class="notifications-component-dialog-overlay"></div>
      </details>
    </notifications-list-subscription-form>



  </li>

  <li>
        <div data-view-component="true" class="BtnGroup">
        <button icon="repo-forked" aria-label="Cannot fork because you own this repository and are not a member of any organizations." disabled="disabled" type="button" data-view-component="true" class="tooltipped tooltipped-s btn-sm btn BtnGroup-item">    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-repo-forked mr-2">
    <path fill-rule="evenodd" d="M5 3.25a.75.75 0 11-1.5 0 .75.75 0 011.5 0zm0 2.122a2.25 2.25 0 10-1.5 0v.878A2.25 2.25 0 005.75 8.5h1.5v2.128a2.251 2.251 0 101.5 0V8.5h1.5a2.25 2.25 0 002.25-2.25v-.878a2.25 2.25 0 10-1.5 0v.878a.75.75 0 01-.75.75h-4.5A.75.75 0 015 6.25v-.878zm3.75 7.378a.75.75 0 11-1.5 0 .75.75 0 011.5 0zm3-8.75a.75.75 0 100-1.5.75.75 0 000 1.5z"></path>
</svg>Fork
        <span id="repo-network-counter" data-pjax-replace="true" data-turbo-replace="true" title="71" data-view-component="true" class="Counter">71</span>
</button>
      <details group_item="true" id="my-forks-menu-575813281" data-view-component="true" class="details-reset details-overlay BtnGroup-parent d-inline-block position-relative">
              <summary aria-label="See your forks of this repository" data-view-component="true" class="btn-sm btn BtnGroup-item px-2 float-none">    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-triangle-down">
    <path d="M4.427 7.427l3.396 3.396a.25.25 0 00.354 0l3.396-3.396A.25.25 0 0011.396 7H4.604a.25.25 0 00-.177.427z"></path>
</svg>
</summary>
  <details-menu
    class="SelectMenu right-0"
      src="/sean207cc/AI-course/my_forks_menu_content?can_fork=false"
      
      role="menu"
      
>
    <div class="SelectMenu-modal">
        <button class="SelectMenu-closeButton position-absolute right-0 m-2" type="button" aria-label="Close menu" data-toggle-for="details-e1561c">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path>
</svg>
        </button>
      <div
        id="filter-menu-e1561c"
        class="d-flex flex-column flex-1 overflow-hidden"
>
        <div
          class="SelectMenu-list"
          >

            <include-fragment class="SelectMenu-loading" aria-label="Loading">
              <svg role="menuitem" style="box-sizing: content-box; color: var(--color-icon-primary);" width="32" height="32" viewBox="0 0 16 16" fill="none" data-view-component="true" class="anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" />
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke" />
</svg>
            </include-fragment>
        </div>
        
      </div>
    </div>
  </details-menu>
</details></div>
  </li>

  <li>
        <template class="js-unstar-confirmation-dialog-template">
  <div class="Box-header">
    <h2 class="Box-title">Unstar this repository?</h2>
  </div>
  <div class="Box-body">
    <p class="mb-3">
      This will remove {{ repoNameWithOwner }} from the {{ listsWithCount }} that it's been added to.
    </p>
    <div class="form-actions">
      <form class="js-social-confirmation-form" data-turbo="false" action="{{ confirmUrl }}" accept-charset="UTF-8" method="post">
        <input type="hidden" name="authenticity_token" value="{{ confirmCsrfToken }}">
        <input type="hidden" name="confirm" value="true">
          <button data-close-dialog="true" type="submit" data-view-component="true" class="btn-danger btn width-full">    Unstar
</button>
</form>    </div>
  </div>
</template>

  <div data-view-component="true" class="js-toggler-container js-social-container starring-container d-flex">
    <div data-view-component="true" class="starred BtnGroup flex-1">
      <form class="js-social-form BtnGroup-parent flex-auto js-deferred-toggler-target" data-turbo="false" action="/sean207cc/AI-course/unstar" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="MsCQlmb2xEt6INcdbkLKJ2cGUjdqYlC1Lfj0F4UnfKZgfRS78SqxILvOQFJc-qyGij24ek5jdsaVSJIMD0922w" autocomplete="off" />
          <input type="hidden" value="zclP76NurrDQG-LeEDDfWRO5dlDFgPXEboFYv0iDYaGfdMvCNLLb2xH1dZEiiLn4_oKcHeGB07fWMT6kwutr3A" data-csrf="true" class="js-confirm-csrf-token" />
        <input type="hidden" name="context" value="repository">
          <button data-hydro-click="{&quot;event_type&quot;:&quot;repository.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;UNSTAR_BUTTON&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afe39bf8c51d3663543fc2af3412199d6cef675cc681216ebf5d08ba65b98f99" data-ga-click="Repository, click unstar button, action:blob#show; text:Unstar" aria-label="Unstar this repository (0)" type="submit" data-view-component="true" class="rounded-left-2 btn-sm btn BtnGroup-item">    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-star-fill starred-button-icon d-inline-block mr-2">
    <path fill-rule="evenodd" d="M8 .25a.75.75 0 01.673.418l1.882 3.815 4.21.612a.75.75 0 01.416 1.279l-3.046 2.97.719 4.192a.75.75 0 01-1.088.791L8 12.347l-3.766 1.98a.75.75 0 01-1.088-.79l.72-4.194L.818 6.374a.75.75 0 01.416-1.28l4.21-.611L7.327.668A.75.75 0 018 .25z"></path>
</svg><span data-view-component="true" class="d-inline">
            Starred
</span>            <span id="repo-stars-counter-unstar" aria-label="0 users starred this repository" data-singular-suffix="user starred this repository" data-plural-suffix="users starred this repository" data-turbo-replace="true" title="0" data-view-component="true" class="Counter js-social-count">0</span>
</button></form>        <details id="details-user-list-575813281" data-view-component="true" class="details-reset details-overlay BtnGroup-parent js-user-list-menu d-inline-block position-relative">
        <summary aria-label="Add this repository to a list" data-view-component="true" class="btn-sm btn BtnGroup-item px-2 float-none">    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-triangle-down">
    <path d="M4.427 7.427l3.396 3.396a.25.25 0 00.354 0l3.396-3.396A.25.25 0 0011.396 7H4.604a.25.25 0 00-.177.427z"></path>
</svg>
</summary>
  <details-menu
    class="SelectMenu right-0"
      src="/sean207cc/AI-course/lists"
      
      role="menu"
      
>
    <div class="SelectMenu-modal">
        <button class="SelectMenu-closeButton position-absolute right-0 m-2" type="button" aria-label="Close menu" data-toggle-for="details-ddedea">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path>
</svg>
        </button>
      <div
        id="filter-menu-ddedea"
        class="d-flex flex-column flex-1 overflow-hidden"
>
        <div
          class="SelectMenu-list"
          >

            <include-fragment class="SelectMenu-loading" aria-label="Loading">
              <svg role="menuitem" style="box-sizing: content-box; color: var(--color-icon-primary);" width="32" height="32" viewBox="0 0 16 16" fill="none" data-view-component="true" class="anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" />
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke" />
</svg>
            </include-fragment>
        </div>
        
      </div>
    </div>
  </details-menu>
</details>
</div>
    <div data-view-component="true" class="unstarred BtnGroup flex-1">
      <form class="js-social-form BtnGroup-parent flex-auto" data-turbo="false" action="/sean207cc/AI-course/star" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="xygDGuClAH1rIRoqWOwnBimRHhQTSR2ae5AbyGZgrD67AIeak-xReFyenjvOI97xjcUy2pvAWbUZlx2Re3Mvsg" autocomplete="off" />
        <input type="hidden" name="context" value="repository">
          <button data-hydro-click="{&quot;event_type&quot;:&quot;repository.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;STAR_BUTTON&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="69136efe5402cce496a641ede09d70f611a3560796a6064d6a1fd0d359734cb4" data-ga-click="Repository, click star button, action:blob#show; text:Star" aria-label="Star this repository (0)" type="submit" data-view-component="true" class="js-toggler-target rounded-left-2 btn-sm btn BtnGroup-item">    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-star d-inline-block mr-2">
    <path fill-rule="evenodd" d="M8 .25a.75.75 0 01.673.418l1.882 3.815 4.21.612a.75.75 0 01.416 1.279l-3.046 2.97.719 4.192a.75.75 0 01-1.088.791L8 12.347l-3.766 1.98a.75.75 0 01-1.088-.79l.72-4.194L.818 6.374a.75.75 0 01.416-1.28l4.21-.611L7.327.668A.75.75 0 018 .25zm0 2.445L6.615 5.5a.75.75 0 01-.564.41l-3.097.45 2.24 2.184a.75.75 0 01.216.664l-.528 3.084 2.769-1.456a.75.75 0 01.698 0l2.77 1.456-.53-3.084a.75.75 0 01.216-.664l2.24-2.183-3.096-.45a.75.75 0 01-.564-.41L8 2.694v.001z"></path>
</svg><span data-view-component="true" class="d-inline">
            Star
</span>            <span id="repo-stars-counter-star" aria-label="0 users starred this repository" data-singular-suffix="user starred this repository" data-plural-suffix="users starred this repository" data-turbo-replace="true" title="0" data-view-component="true" class="Counter js-social-count">0</span>
</button></form>        <details id="details-user-list-575813281" data-view-component="true" class="details-reset details-overlay BtnGroup-parent js-user-list-menu d-inline-block position-relative">
        <summary aria-label="Add this repository to a list" data-view-component="true" class="btn-sm btn BtnGroup-item px-2 float-none">    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-triangle-down">
    <path d="M4.427 7.427l3.396 3.396a.25.25 0 00.354 0l3.396-3.396A.25.25 0 0011.396 7H4.604a.25.25 0 00-.177.427z"></path>
</svg>
</summary>
  <details-menu
    class="SelectMenu right-0"
      src="/sean207cc/AI-course/lists"
      
      role="menu"
      
>
    <div class="SelectMenu-modal">
        <button class="SelectMenu-closeButton position-absolute right-0 m-2" type="button" aria-label="Close menu" data-toggle-for="details-ddedea">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path>
</svg>
        </button>
      <div
        id="filter-menu-ddedea"
        class="d-flex flex-column flex-1 overflow-hidden"
>
        <div
          class="SelectMenu-list"
          >

            <include-fragment class="SelectMenu-loading" aria-label="Loading">
              <svg role="menuitem" style="box-sizing: content-box; color: var(--color-icon-primary);" width="32" height="32" viewBox="0 0 16 16" fill="none" data-view-component="true" class="anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" />
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke" />
</svg>
            </include-fragment>
        </div>
        
      </div>
    </div>
  </details-menu>
</details>
</div></div>
  </li>

    

</ul>

      </div>

        <div id="responsive-meta-container" data-turbo-replace>
</div>


          <nav data-pjax="#js-repo-pjax-container" aria-label="Repository" data-view-component="true" class="js-repo-nav js-sidenav-container-pjax js-responsive-underlinenav overflow-hidden UnderlineNav px-3 px-md-4 px-lg-5">

  <ul data-view-component="true" class="UnderlineNav-body list-style-none">
      <li data-view-component="true" class="d-inline-flex">
  <a id="code-tab" href="/sean207cc/AI-course" data-tab-item="i0code-tab" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches repo_packages repo_deployments /sean207cc/AI-course" data-pjax="#repo-content-pjax-container" data-turbo-frame="repo-content-turbo-frame" data-hotkey="g c" data-analytics-event="{&quot;category&quot;:&quot;Underline navbar&quot;,&quot;action&quot;:&quot;Click tab&quot;,&quot;label&quot;:&quot;Code&quot;,&quot;target&quot;:&quot;UNDERLINE_NAV.TAB&quot;}" aria-current="page" data-view-component="true" class="UnderlineNav-item no-wrap js-responsive-underlinenav-item js-selected-navigation-item selected">
    
                <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-code UnderlineNav-octicon d-none d-sm-inline">
    <path fill-rule="evenodd" d="M4.72 3.22a.75.75 0 011.06 1.06L2.06 8l3.72 3.72a.75.75 0 11-1.06 1.06L.47 8.53a.75.75 0 010-1.06l4.25-4.25zm6.56 0a.75.75 0 10-1.06 1.06L13.94 8l-3.72 3.72a.75.75 0 101.06 1.06l4.25-4.25a.75.75 0 000-1.06l-4.25-4.25z"></path>
</svg>
        <span data-content="Code">Code</span>
          <span id="code-repo-tab-count" data-pjax-replace="" data-turbo-replace="" title="Not available" data-view-component="true" class="Counter"></span>


    
</a></li>
      <li data-view-component="true" class="d-inline-flex">
  <a id="pull-requests-tab" href="/sean207cc/AI-course/pulls" data-tab-item="i1pull-requests-tab" data-selected-links="repo_pulls checks /sean207cc/AI-course/pulls" data-pjax="#repo-content-pjax-container" data-turbo-frame="repo-content-turbo-frame" data-hotkey="g p" data-analytics-event="{&quot;category&quot;:&quot;Underline navbar&quot;,&quot;action&quot;:&quot;Click tab&quot;,&quot;label&quot;:&quot;Pull requests&quot;,&quot;target&quot;:&quot;UNDERLINE_NAV.TAB&quot;}" data-view-component="true" class="UnderlineNav-item no-wrap js-responsive-underlinenav-item js-selected-navigation-item">
    
                <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-git-pull-request UnderlineNav-octicon d-none d-sm-inline">
    <path fill-rule="evenodd" d="M7.177 3.073L9.573.677A.25.25 0 0110 .854v4.792a.25.25 0 01-.427.177L7.177 3.427a.25.25 0 010-.354zM3.75 2.5a.75.75 0 100 1.5.75.75 0 000-1.5zm-2.25.75a2.25 2.25 0 113 2.122v5.256a2.251 2.251 0 11-1.5 0V5.372A2.25 2.25 0 011.5 3.25zM11 2.5h-1V4h1a1 1 0 011 1v5.628a2.251 2.251 0 101.5 0V5A2.5 2.5 0 0011 2.5zm1 10.25a.75.75 0 111.5 0 .75.75 0 01-1.5 0zM3.75 12a.75.75 0 100 1.5.75.75 0 000-1.5z"></path>
</svg>
        <span data-content="Pull requests">Pull requests</span>
          <span id="pull-requests-repo-tab-count" data-pjax-replace="" data-turbo-replace="" title="0" hidden="hidden" data-view-component="true" class="Counter">0</span>


    
</a></li>
      <li data-view-component="true" class="d-inline-flex">
  <a id="actions-tab" href="/sean207cc/AI-course/actions" data-tab-item="i2actions-tab" data-selected-links="repo_actions /sean207cc/AI-course/actions" data-pjax="#repo-content-pjax-container" data-turbo-frame="repo-content-turbo-frame" data-hotkey="g a" data-analytics-event="{&quot;category&quot;:&quot;Underline navbar&quot;,&quot;action&quot;:&quot;Click tab&quot;,&quot;label&quot;:&quot;Actions&quot;,&quot;target&quot;:&quot;UNDERLINE_NAV.TAB&quot;}" data-view-component="true" class="UnderlineNav-item no-wrap js-responsive-underlinenav-item js-selected-navigation-item">
    
                <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-play UnderlineNav-octicon d-none d-sm-inline">
    <path fill-rule="evenodd" d="M1.5 8a6.5 6.5 0 1113 0 6.5 6.5 0 01-13 0zM8 0a8 8 0 100 16A8 8 0 008 0zM6.379 5.227A.25.25 0 006 5.442v5.117a.25.25 0 00.379.214l4.264-2.559a.25.25 0 000-.428L6.379 5.227z"></path>
</svg>
        <span data-content="Actions">Actions</span>
          <span id="actions-repo-tab-count" data-pjax-replace="" data-turbo-replace="" title="Not available" data-view-component="true" class="Counter"></span>


    
</a></li>
      <li data-view-component="true" class="d-inline-flex">
  <a id="projects-tab" href="/sean207cc/AI-course/projects" data-tab-item="i3projects-tab" data-selected-links="repo_projects new_repo_project repo_project /sean207cc/AI-course/projects" data-pjax="#repo-content-pjax-container" data-turbo-frame="repo-content-turbo-frame" data-hotkey="g b" data-analytics-event="{&quot;category&quot;:&quot;Underline navbar&quot;,&quot;action&quot;:&quot;Click tab&quot;,&quot;label&quot;:&quot;Projects&quot;,&quot;target&quot;:&quot;UNDERLINE_NAV.TAB&quot;}" data-view-component="true" class="UnderlineNav-item no-wrap js-responsive-underlinenav-item js-selected-navigation-item">
    
                <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-table UnderlineNav-octicon d-none d-sm-inline">
    <path fill-rule="evenodd" d="M0 1.75C0 .784.784 0 1.75 0h12.5C15.216 0 16 .784 16 1.75v12.5A1.75 1.75 0 0114.25 16H1.75A1.75 1.75 0 010 14.25V1.75zM1.5 6.5v7.75c0 .138.112.25.25.25H5v-8H1.5zM5 5H1.5V1.75a.25.25 0 01.25-.25H5V5zm1.5 1.5v8h7.75a.25.25 0 00.25-.25V6.5h-8zm8-1.5h-8V1.5h7.75a.25.25 0 01.25.25V5z"></path>
</svg>
        <span data-content="Projects">Projects</span>
          <span id="projects-repo-tab-count" data-pjax-replace="" data-turbo-replace="" title="0" hidden="hidden" data-view-component="true" class="Counter">0</span>


    
</a></li>
      <li data-view-component="true" class="d-inline-flex">
  <a id="wiki-tab" href="/sean207cc/AI-course/wiki" data-tab-item="i4wiki-tab" data-selected-links="repo_wiki /sean207cc/AI-course/wiki" data-pjax="#repo-content-pjax-container" data-turbo-frame="repo-content-turbo-frame" data-hotkey="g w" data-analytics-event="{&quot;category&quot;:&quot;Underline navbar&quot;,&quot;action&quot;:&quot;Click tab&quot;,&quot;label&quot;:&quot;Wiki&quot;,&quot;target&quot;:&quot;UNDERLINE_NAV.TAB&quot;}" data-view-component="true" class="UnderlineNav-item no-wrap js-responsive-underlinenav-item js-selected-navigation-item">
    
                <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-book UnderlineNav-octicon d-none d-sm-inline">
    <path fill-rule="evenodd" d="M0 1.75A.75.75 0 01.75 1h4.253c1.227 0 2.317.59 3 1.501A3.744 3.744 0 0111.006 1h4.245a.75.75 0 01.75.75v10.5a.75.75 0 01-.75.75h-4.507a2.25 2.25 0 00-1.591.659l-.622.621a.75.75 0 01-1.06 0l-.622-.621A2.25 2.25 0 005.258 13H.75a.75.75 0 01-.75-.75V1.75zm8.755 3a2.25 2.25 0 012.25-2.25H14.5v9h-3.757c-.71 0-1.4.201-1.992.572l.004-7.322zm-1.504 7.324l.004-5.073-.002-2.253A2.25 2.25 0 005.003 2.5H1.5v9h3.757a3.75 3.75 0 011.994.574z"></path>
</svg>
        <span data-content="Wiki">Wiki</span>
          <span id="wiki-repo-tab-count" data-pjax-replace="" data-turbo-replace="" title="Not available" data-view-component="true" class="Counter"></span>


    
</a></li>
      <li data-view-component="true" class="d-inline-flex">
  <a id="security-tab" href="/sean207cc/AI-course/security" data-tab-item="i5security-tab" data-selected-links="security overview alerts policy token_scanning code_scanning /sean207cc/AI-course/security" data-pjax="#repo-content-pjax-container" data-turbo-frame="repo-content-turbo-frame" data-hotkey="g s" data-analytics-event="{&quot;category&quot;:&quot;Underline navbar&quot;,&quot;action&quot;:&quot;Click tab&quot;,&quot;label&quot;:&quot;Security&quot;,&quot;target&quot;:&quot;UNDERLINE_NAV.TAB&quot;}" data-view-component="true" class="UnderlineNav-item no-wrap js-responsive-underlinenav-item js-selected-navigation-item">
    
                <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-shield UnderlineNav-octicon d-none d-sm-inline">
    <path fill-rule="evenodd" d="M7.467.133a1.75 1.75 0 011.066 0l5.25 1.68A1.75 1.75 0 0115 3.48V7c0 1.566-.32 3.182-1.303 4.682-.983 1.498-2.585 2.813-5.032 3.855a1.7 1.7 0 01-1.33 0c-2.447-1.042-4.049-2.357-5.032-3.855C1.32 10.182 1 8.566 1 7V3.48a1.75 1.75 0 011.217-1.667l5.25-1.68zm.61 1.429a.25.25 0 00-.153 0l-5.25 1.68a.25.25 0 00-.174.238V7c0 1.358.275 2.666 1.057 3.86.784 1.194 2.121 2.34 4.366 3.297a.2.2 0 00.154 0c2.245-.956 3.582-2.104 4.366-3.298C13.225 9.666 13.5 8.36 13.5 7V3.48a.25.25 0 00-.174-.237l-5.25-1.68zM9 10.5a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.75a.75.75 0 10-1.5 0v3a.75.75 0 001.5 0v-3z"></path>
</svg>
        <span data-content="Security">Security</span>
          <include-fragment src="/sean207cc/AI-course/security/overall-count" accept="text/fragment+html"></include-fragment>

    
</a></li>
      <li data-view-component="true" class="d-inline-flex">
  <a id="insights-tab" href="/sean207cc/AI-course/pulse" data-tab-item="i6insights-tab" data-selected-links="repo_graphs repo_contributors dependency_graph dependabot_updates pulse people community /sean207cc/AI-course/pulse" data-pjax="#repo-content-pjax-container" data-turbo-frame="repo-content-turbo-frame" data-analytics-event="{&quot;category&quot;:&quot;Underline navbar&quot;,&quot;action&quot;:&quot;Click tab&quot;,&quot;label&quot;:&quot;Insights&quot;,&quot;target&quot;:&quot;UNDERLINE_NAV.TAB&quot;}" data-view-component="true" class="UnderlineNav-item no-wrap js-responsive-underlinenav-item js-selected-navigation-item">
    
                <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-graph UnderlineNav-octicon d-none d-sm-inline">
    <path fill-rule="evenodd" d="M1.5 1.75a.75.75 0 00-1.5 0v12.5c0 .414.336.75.75.75h14.5a.75.75 0 000-1.5H1.5V1.75zm14.28 2.53a.75.75 0 00-1.06-1.06L10 7.94 7.53 5.47a.75.75 0 00-1.06 0L3.22 8.72a.75.75 0 001.06 1.06L7 7.06l2.47 2.47a.75.75 0 001.06 0l5.25-5.25z"></path>
</svg>
        <span data-content="Insights">Insights</span>
          <span id="insights-repo-tab-count" data-pjax-replace="" data-turbo-replace="" title="Not available" data-view-component="true" class="Counter"></span>


    
</a></li>
      <li data-view-component="true" class="d-inline-flex">
  <a id="settings-tab" href="/sean207cc/AI-course/settings" data-tab-item="i7settings-tab" data-selected-links="code_review_limits codespaces_repository_settings collaborators custom_tabs hooks integration_installations interaction_limits issue_template_editor key_links_settings notifications repo_actions_settings repo_announcements repo_branch_settings repo_keys_settings repo_pages_settings repo_rulesets repo_protected_tags_settings repo_settings reported_content repository_actions_settings_add_new_runner repository_actions_settings_general repository_actions_settings_runners repository_environments role_details secrets_settings_actions secrets_settings_codespaces secrets_settings_dependabot security_analysis /sean207cc/AI-course/settings" data-pjax="#repo-content-pjax-container" data-turbo-frame="repo-content-turbo-frame" data-analytics-event="{&quot;category&quot;:&quot;Underline navbar&quot;,&quot;action&quot;:&quot;Click tab&quot;,&quot;label&quot;:&quot;Settings&quot;,&quot;target&quot;:&quot;UNDERLINE_NAV.TAB&quot;}" data-view-component="true" class="UnderlineNav-item no-wrap js-responsive-underlinenav-item js-selected-navigation-item">
    
                <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-gear UnderlineNav-octicon d-none d-sm-inline">
    <path fill-rule="evenodd" d="M7.429 1.525a6.593 6.593 0 011.142 0c.036.003.108.036.137.146l.289 1.105c.147.56.55.967.997 1.189.174.086.341.183.501.29.417.278.97.423 1.53.27l1.102-.303c.11-.03.175.016.195.046.219.31.41.641.573.989.014.031.022.11-.059.19l-.815.806c-.411.406-.562.957-.53 1.456a4.588 4.588 0 010 .582c-.032.499.119 1.05.53 1.456l.815.806c.08.08.073.159.059.19a6.494 6.494 0 01-.573.99c-.02.029-.086.074-.195.045l-1.103-.303c-.559-.153-1.112-.008-1.529.27-.16.107-.327.204-.5.29-.449.222-.851.628-.998 1.189l-.289 1.105c-.029.11-.101.143-.137.146a6.613 6.613 0 01-1.142 0c-.036-.003-.108-.037-.137-.146l-.289-1.105c-.147-.56-.55-.967-.997-1.189a4.502 4.502 0 01-.501-.29c-.417-.278-.97-.423-1.53-.27l-1.102.303c-.11.03-.175-.016-.195-.046a6.492 6.492 0 01-.573-.989c-.014-.031-.022-.11.059-.19l.815-.806c.411-.406.562-.957.53-1.456a4.587 4.587 0 010-.582c.032-.499-.119-1.05-.53-1.456l-.815-.806c-.08-.08-.073-.159-.059-.19a6.44 6.44 0 01.573-.99c.02-.029.086-.075.195-.045l1.103.303c.559.153 1.112.008 1.529-.27.16-.107.327-.204.5-.29.449-.222.851-.628.998-1.189l.289-1.105c.029-.11.101-.143.137-.146zM8 0c-.236 0-.47.01-.701.03-.743.065-1.29.615-1.458 1.261l-.29 1.106c-.017.066-.078.158-.211.224a5.994 5.994 0 00-.668.386c-.123.082-.233.09-.3.071L3.27 2.776c-.644-.177-1.392.02-1.82.63a7.977 7.977 0 00-.704 1.217c-.315.675-.111 1.422.363 1.891l.815.806c.05.048.098.147.088.294a6.084 6.084 0 000 .772c.01.147-.038.246-.088.294l-.815.806c-.474.469-.678 1.216-.363 1.891.2.428.436.835.704 1.218.428.609 1.176.806 1.82.63l1.103-.303c.066-.019.176-.011.299.071.213.143.436.272.668.386.133.066.194.158.212.224l.289 1.106c.169.646.715 1.196 1.458 1.26a8.094 8.094 0 001.402 0c.743-.064 1.29-.614 1.458-1.26l.29-1.106c.017-.066.078-.158.211-.224a5.98 5.98 0 00.668-.386c.123-.082.233-.09.3-.071l1.102.302c.644.177 1.392-.02 1.82-.63.268-.382.505-.789.704-1.217.315-.675.111-1.422-.364-1.891l-.814-.806c-.05-.048-.098-.147-.088-.294a6.1 6.1 0 000-.772c-.01-.147.039-.246.088-.294l.814-.806c.475-.469.679-1.216.364-1.891a7.992 7.992 0 00-.704-1.218c-.428-.609-1.176-.806-1.82-.63l-1.103.303c-.066.019-.176.011-.299-.071a5.991 5.991 0 00-.668-.386c-.133-.066-.194-.158-.212-.224L10.16 1.29C9.99.645 9.444.095 8.701.031A8.094 8.094 0 008 0zm1.5 8a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0zM11 8a3 3 0 11-6 0 3 3 0 016 0z"></path>
</svg>
        <span data-content="Settings">Settings</span>
          <span id="settings-repo-tab-count" data-pjax-replace="" data-turbo-replace="" title="Not available" data-view-component="true" class="Counter"></span>


    
</a></li>
</ul>
    <div style="visibility:hidden;" data-view-component="true" class="UnderlineNav-actions js-responsive-underlinenav-overflow position-absolute pr-3 pr-md-4 pr-lg-5 right-0">      <details data-view-component="true" class="details-overlay details-reset position-relative">
  <summary role="button" data-view-component="true">          <div class="UnderlineNav-item mr-0 border-0">
            <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-kebab-horizontal">
    <path d="M8 9a1.5 1.5 0 100-3 1.5 1.5 0 000 3zM1.5 9a1.5 1.5 0 100-3 1.5 1.5 0 000 3zm13 0a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path>
</svg>
            <span class="sr-only">More</span>
          </div>
</summary>
  <details-menu role="menu" data-view-component="true" class="dropdown-menu dropdown-menu-sw">          <ul>
              <li data-menu-item="i0code-tab" hidden>
                <a role="menuitem" class="js-selected-navigation-item selected dropdown-item" aria-current="page" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches repo_packages repo_deployments /sean207cc/AI-course" href="/sean207cc/AI-course">
                  Code
</a>              </li>
              <li data-menu-item="i1pull-requests-tab" hidden>
                <a role="menuitem" class="js-selected-navigation-item dropdown-item" data-selected-links="repo_pulls checks /sean207cc/AI-course/pulls" href="/sean207cc/AI-course/pulls">
                  Pull requests
</a>              </li>
              <li data-menu-item="i2actions-tab" hidden>
                <a role="menuitem" class="js-selected-navigation-item dropdown-item" data-selected-links="repo_actions /sean207cc/AI-course/actions" href="/sean207cc/AI-course/actions">
                  Actions
</a>              </li>
              <li data-menu-item="i3projects-tab" hidden>
                <a role="menuitem" class="js-selected-navigation-item dropdown-item" data-selected-links="repo_projects new_repo_project repo_project /sean207cc/AI-course/projects" href="/sean207cc/AI-course/projects">
                  Projects
</a>              </li>
              <li data-menu-item="i4wiki-tab" hidden>
                <a role="menuitem" class="js-selected-navigation-item dropdown-item" data-selected-links="repo_wiki /sean207cc/AI-course/wiki" href="/sean207cc/AI-course/wiki">
                  Wiki
</a>              </li>
              <li data-menu-item="i5security-tab" hidden>
                <a role="menuitem" class="js-selected-navigation-item dropdown-item" data-selected-links="security overview alerts policy token_scanning code_scanning /sean207cc/AI-course/security" href="/sean207cc/AI-course/security">
                  Security
</a>              </li>
              <li data-menu-item="i6insights-tab" hidden>
                <a role="menuitem" class="js-selected-navigation-item dropdown-item" data-selected-links="repo_graphs repo_contributors dependency_graph dependabot_updates pulse people community /sean207cc/AI-course/pulse" href="/sean207cc/AI-course/pulse">
                  Insights
</a>              </li>
              <li data-menu-item="i7settings-tab" hidden>
                <a role="menuitem" class="js-selected-navigation-item dropdown-item" data-selected-links="code_review_limits codespaces_repository_settings collaborators custom_tabs hooks integration_installations interaction_limits issue_template_editor key_links_settings notifications repo_actions_settings repo_announcements repo_branch_settings repo_keys_settings repo_pages_settings repo_rulesets repo_protected_tags_settings repo_settings reported_content repository_actions_settings_add_new_runner repository_actions_settings_general repository_actions_settings_runners repository_environments role_details secrets_settings_actions secrets_settings_codespaces secrets_settings_dependabot security_analysis /sean207cc/AI-course/settings" href="/sean207cc/AI-course/settings">
                  Settings
</a>              </li>
          </ul>
</details-menu>
</details></div>
</nav>

  </div>

  



  <turbo-frame id="repo-content-turbo-frame" target="_top" data-turbo-action="advance" class="">
      <div id="repo-content-pjax-container" class="repository-content " >
      <a href="https://github.dev/" class="d-none js-github-dev-shortcut" data-hotkey=".">Open in github.dev</a>
  <a href="https://github.dev/" class="d-none js-github-dev-new-tab-shortcut" data-hotkey="Shift+.,Shift+&gt;,&gt;" target="_blank">Open in a new github.dev tab</a>



    
      
  <div class="clearfix container-xl px-3 px-md-4 px-lg-5 mt-4">
    
    
<div data-test-selector="blob-container">
  

  



    
<a class="d-none js-permalink-shortcut" data-hotkey="y" href="/sean207cc/AI-course/blob/40389cfbf5b975c899afa75d854d60d2d9e4c7c5/_posts/2022-12-08-Pose-Estimation.md">Permalink</a>

<div class="d-flex flex-items-start flex-shrink-0 pb-3 flex-wrap flex-md-nowrap flex-justify-between flex-md-justify-start">
  
<div class="position-relative">
  <details
    class="js-branch-select-menu details-reset details-overlay mr-0 mb-0 "
    id="branch-select-menu"
    data-hydro-click-payload="{&quot;event_type&quot;:&quot;repository.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;REFS_SELECTOR_MENU&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="01bcc9b9b6d764c8910b5983290f3d34cf71dab563dcfce64186e2557cf24171">
    <summary class="btn css-truncate"
            data-hotkey="w"
            title="Switch branches or tags">
      <svg text="gray" aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-git-branch">
    <path fill-rule="evenodd" d="M11.75 2.5a.75.75 0 100 1.5.75.75 0 000-1.5zm-2.25.75a2.25 2.25 0 113 2.122V6A2.5 2.5 0 0110 8.5H6a1 1 0 00-1 1v1.128a2.251 2.251 0 11-1.5 0V5.372a2.25 2.25 0 111.5 0v1.836A2.492 2.492 0 016 7h4a1 1 0 001-1v-.628A2.25 2.25 0 019.5 3.25zM4.25 12a.75.75 0 100 1.5.75.75 0 000-1.5zM3.5 3.25a.75.75 0 111.5 0 .75.75 0 01-1.5 0z"></path>
</svg>
      <span class="css-truncate-target" data-menu-button>gh-pages</span>
      <span class="dropdown-caret"></span>
    </summary>

    
<div class="SelectMenu">
  <div class="SelectMenu-modal">
    <header class="SelectMenu-header">
      <span class="SelectMenu-title">Switch branches/tags</span>
      <button class="SelectMenu-closeButton" type="button" data-toggle-for="branch-select-menu"><svg aria-label="Close menu" aria-hidden="false" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path>
</svg></button>
    </header>

    <input-demux data-action="tab-container-change:input-demux#storeInput tab-container-changed:input-demux#updateInput">
      <tab-container class="d-flex flex-column js-branches-tags-tabs" style="min-height: 0;">
        <div class="SelectMenu-filter">
          <input data-target="input-demux.source"
                 id="context-commitish-filter-field"
                 class="SelectMenu-input form-control"
                 aria-owns="ref-list-branches"
                 data-controls-ref-menu-id="ref-list-branches"
                 autofocus
                 autocomplete="off"
                 aria-label="Find or create a branch…"
                 placeholder="Find or create a branch…"
                 type="text"
          >
        </div>

        <div class="SelectMenu-tabs" role="tablist" data-target="input-demux.control" >
          <button class="SelectMenu-tab" type="button" role="tab" aria-selected="true">Branches</button>
          <button class="SelectMenu-tab" type="button" role="tab">Tags</button>
        </div>

        <div role="tabpanel" id="ref-list-branches" data-filter-placeholder="Find or create a branch…" tabindex="" class="d-flex flex-column flex-auto overflow-auto">
          <ref-selector
            type="branch"
            data-targets="input-demux.sinks"
            data-action="
              input-entered:ref-selector#inputEntered
              tab-selected:ref-selector#tabSelected
              focus-list:ref-selector#focusFirstListMember
            "
            query-endpoint="/sean207cc/AI-course/refs"
            can-create
            cache-key="v0:1670497394.148412"
            current-committish="Z2gtcGFnZXM="
            default-branch="Z2gtcGFnZXM="
            name-with-owner="c2VhbjIwN2NjL0FJLWNvdXJzZQ=="
            prefetch-on-mouseover
          >

            <template data-target="ref-selector.fetchFailedTemplate">
              <div class="SelectMenu-message" data-index="{{ index }}">Could not load branches</div>
            </template>

              <template data-target="ref-selector.noMatchTemplate">
    <create-repo-from-selector
      check-tag-name-exists-path="/sean207cc/AI-course/branches/check_tag_name_exists"
    >
      <!-- '"` --><!-- </textarea></xmp> --></option></form><form data-turbo="false" action="/sean207cc/AI-course/branches" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="QxarL3LIdQGcme_6w_R04XKpABa1l1a86BmXVR_lo_ccNhXVm9AxHCKWsdkf5DXfMJkTAhW_4i65V_deayZvvg" />
        <input data-target="create-repo-from-selector.refName" type="hidden" name="name" value="{{ refName }}">
        <input type="hidden" name="branch"  value="gh-pages">
        <input type="hidden" name="path_binary" value="X3Bvc3RzLzIwMjItMTItMDgtUG9zZS1Fc3RpbWF0aW9uLm1k">

        <button
          class="SelectMenu-item wb-break-word"
          type="submit"
          role="menuitem"
          data-index="{{ index }}"
          data-action="click:create-repo-from-selector#createBranch"
          data-hydro-click="{&quot;event_type&quot;:&quot;repository.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;REFS_SELECTOR_MENU_CREATE_BRANCH&quot;,&quot;repository_id&quot;:575813281,&quot;ref_name&quot;:&quot;{{ refName }}&quot;,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="9ec1054d68c688c071690950d750a6474c64328f1e596e6f7027df00ac1f581e">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-git-branch SelectMenu-icon flex-self-baseline">
    <path fill-rule="evenodd" d="M11.75 2.5a.75.75 0 100 1.5.75.75 0 000-1.5zm-2.25.75a2.25 2.25 0 113 2.122V6A2.5 2.5 0 0110 8.5H6a1 1 0 00-1 1v1.128a2.251 2.251 0 11-1.5 0V5.372a2.25 2.25 0 111.5 0v1.836A2.492 2.492 0 016 7h4a1 1 0 001-1v-.628A2.25 2.25 0 019.5 3.25zM4.25 12a.75.75 0 100 1.5.75.75 0 000-1.5zM3.5 3.25a.75.75 0 111.5 0 .75.75 0 01-1.5 0z"></path>
</svg>
          <div>
            <span class="text-bold">Create branch: {{ refName }}</span>
            <span class="color-fg-muted">from ‘gh-pages’</span>
            <input type="hidden" value="E1oV3LM3stAHEdJQfoWTyDUBrEzCeldI_27cPjLQeZT7MVuRiNxP6piqprx8UUC5YCQmS-6cA8tuKIFzKAOX-Q" data-csrf="true" data-target="create-repo-from-selector.checkTagNameExistsPathCsrf" />
          </div>
        </button>
</form>    </create-repo-from-selector>
</template>


            <div data-target="ref-selector.listContainer" role="menu" class="SelectMenu-list " data-turbo-frame="repo-content-turbo-frame">
              <div class="SelectMenu-loading pt-3 pb-0 overflow-hidden" aria-label="Menu is loading">
                <svg style="box-sizing: content-box; color: var(--color-icon-primary);" width="32" height="32" viewBox="0 0 16 16" fill="none" data-view-component="true" class="anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" />
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke" />
</svg>
              </div>
            </div>

              

<template data-target="ref-selector.itemTemplate">
  <a href="https://github.com/sean207cc/AI-course/blob/{{ urlEncodedRefName }}/_posts/2022-12-08-Pose-Estimation.md" class="SelectMenu-item" role="menuitemradio" rel="nofollow" aria-checked="{{ isCurrent }}" data-index="{{ index }}" >
    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check SelectMenu-icon SelectMenu-icon--check">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
    <span class="flex-1 css-truncate css-truncate-overflow {{ isFilteringClass }}">{{ refName }}</span>
    <span hidden="{{ isNotDefault }}" class="Label Label--secondary flex-self-start">default</span>
  </a>
</template>


              <footer class="SelectMenu-footer"><a href="/sean207cc/AI-course/branches">View all branches</a></footer>
          </ref-selector>

        </div>

        <div role="tabpanel" id="tags-menu" data-filter-placeholder="Find a tag" tabindex="" hidden class="d-flex flex-column flex-auto overflow-auto">
          <ref-selector
            type="tag"
            data-action="
              input-entered:ref-selector#inputEntered
              tab-selected:ref-selector#tabSelected
              focus-list:ref-selector#focusFirstListMember
            "
            data-targets="input-demux.sinks"
            query-endpoint="/sean207cc/AI-course/refs"
            cache-key="v0:1670497394.148412"
            current-committish="Z2gtcGFnZXM="
            default-branch="Z2gtcGFnZXM="
            name-with-owner="c2VhbjIwN2NjL0FJLWNvdXJzZQ=="
          >

            <template data-target="ref-selector.fetchFailedTemplate">
              <div class="SelectMenu-message" data-index="{{ index }}">Could not load tags</div>
            </template>

            <template data-target="ref-selector.noMatchTemplate">
              <div class="SelectMenu-message" data-index="{{ index }}">Nothing to show</div>
            </template>

              

<template data-target="ref-selector.itemTemplate">
  <a href="https://github.com/sean207cc/AI-course/blob/{{ urlEncodedRefName }}/_posts/2022-12-08-Pose-Estimation.md" class="SelectMenu-item" role="menuitemradio" rel="nofollow" aria-checked="{{ isCurrent }}" data-index="{{ index }}" >
    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check SelectMenu-icon SelectMenu-icon--check">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
    <span class="flex-1 css-truncate css-truncate-overflow {{ isFilteringClass }}">{{ refName }}</span>
    <span hidden="{{ isNotDefault }}" class="Label Label--secondary flex-self-start">default</span>
  </a>
</template>


            <div data-target="ref-selector.listContainer" role="menu" class="SelectMenu-list" data-turbo-frame="repo-content-turbo-frame">
              <div class="SelectMenu-loading pt-3 pb-0 overflow-hidden" aria-label="Menu is loading">
                <svg style="box-sizing: content-box; color: var(--color-icon-primary);" width="32" height="32" viewBox="0 0 16 16" fill="none" data-view-component="true" class="anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" />
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke" />
</svg>
              </div>
            </div>
              <footer class="SelectMenu-footer"><a href="/sean207cc/AI-course/tags">View all tags</a></footer>
          </ref-selector>
        </div>
      </tab-container>
    </input-demux>
  </div>
</div>

  </details>

</div>


<div class="Overlay--hidden Overlay-backdrop--center" data-modal-dialog-overlay>
  <modal-dialog role="dialog" id="warn-tag-match-create-branch-dialog" aria-modal="true" aria-labelledby="warn-tag-match-create-branch-dialog-header" data-view-component="true" class="Overlay Overlay--width-large Overlay--height-auto Overlay--motion-scaleFade">
      <header class="Overlay-header Overlay-header--large Overlay-header--divided">
        <div class="Overlay-headerContentWrap">
          <div class="Overlay-titleWrap">
            <h1 id="warn-tag-match-create-branch-dialog-header" class="Overlay-title">Name already in use</h1>
          </div>
          <div class="Overlay-actionWrap">
            <button data-close-dialog-id="warn-tag-match-create-branch-dialog" aria-label="Close" type="button" data-view-component="true" class="close-button Overlay-closeButton"><svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path>
</svg></button>
          </div>
        </div>
      </header>
    <div class="Overlay-body ">
      
          <div data-view-component="true">      A tag already exists with the provided branch name. Many Git commands accept both tag and branch names, so creating this branch may cause unexpected behavior. Are you sure you want to create this branch?
</div>

    </div>
      <footer class="Overlay-footer Overlay-footer--alignEnd">
            <button data-close-dialog-id="warn-tag-match-create-branch-dialog" type="button" data-view-component="true" class="btn">    Cancel
</button>
            <button data-submit-dialog-id="warn-tag-match-create-branch-dialog" type="button" data-view-component="true" class="btn-danger btn">    Create
</button>
      </footer>
</modal-dialog></div>


  <h2 id="blob-path" class="breadcrumb flex-auto flex-self-center min-width-0 text-normal mx-2 width-full width-md-auto flex-order-1 flex-md-order-none mt-3 mt-md-0">
    <span class="js-repo-root text-bold"><span class="js-path-segment d-inline-block wb-break-all"><a data-turbo-frame="repo-content-turbo-frame" href="/sean207cc/AI-course"><span>AI-course</span></a></span></span><span class="separator">/</span><span class="js-path-segment d-inline-block wb-break-all"><a data-turbo-frame="repo-content-turbo-frame" href="/sean207cc/AI-course/tree/gh-pages/_posts"><span>_posts</span></a></span><span class="separator">/</span><strong class="final-path">2022-12-08-Pose-Estimation.md</strong>
  </h2>
    <a href="/sean207cc/AI-course/find/gh-pages" data-pjax="" data-hotkey="t" data-view-component="true" class="btn mr-2 d-none d-md-block">    Go to file
</a>
  <details id="blob-more-options-details" data-view-component="true" class="details-overlay details-reset position-relative">
    <summary role="button" data-view-component="true" class="btn">    <svg aria-label="More options" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-kebab-horizontal">
    <path d="M8 9a1.5 1.5 0 100-3 1.5 1.5 0 000 3zM1.5 9a1.5 1.5 0 100-3 1.5 1.5 0 000 3zm13 0a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path>
</svg>
</summary>
  <div data-view-component="true">      <ul class="dropdown-menu dropdown-menu-sw">
        <li class="d-block d-md-none">
          <a class="dropdown-item d-flex flex-items-baseline" data-hydro-click="{&quot;event_type&quot;:&quot;repository.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;FIND_FILE_BUTTON&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="a58c826bc69890acc499a43d15b25f73a7ae54d3f425543ec77c296bd17e6e90" data-ga-click="Repository, find file, location:repo overview" data-hotkey="t" href="/sean207cc/AI-course/find/gh-pages">
            <span class="flex-auto">Go to file</span>
            <span class="text-small color-fg-muted" aria-hidden="true">T</span>
</a>        </li>
        <li data-toggle-for="blob-more-options-details">
            <button data-toggle-for="jumpto-line-details-dialog" type="button" data-view-component="true" class="dropdown-item btn-link">    <span class="d-flex flex-items-baseline">
              <span class="flex-auto">Go to line</span>
              <span class="text-small color-fg-muted" aria-hidden="true">L</span>
            </span>
</button>        </li>
        <li class="dropdown-divider" role="none"></li>
        <li>
          <clipboard-copy data-toggle-for="blob-more-options-details" aria-label="Copy path" value="_posts/2022-12-08-Pose-Estimation.md" data-view-component="true" class="dropdown-item cursor-pointer">
    
            Copy path

</clipboard-copy>        </li>
        <li>
          <clipboard-copy data-toggle-for="blob-more-options-details" aria-label="Copy permalink" value="https://github.com/sean207cc/AI-course/blob/40389cfbf5b975c899afa75d854d60d2d9e4c7c5/_posts/2022-12-08-Pose-Estimation.md" data-view-component="true" class="dropdown-item cursor-pointer">
    
            <span class="d-flex flex-items-baseline">
              <span class="flex-auto">Copy permalink</span>
            </span>

</clipboard-copy>        </li>
      </ul>
</div>
</details></div>





    <div id="spoof-warning" class="mt-0 pb-3" hidden aria-hidden>
  <div data-view-component="true" class="flash flash-warn mt-0 clearfix">
  
  
    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-alert float-left mt-1">
    <path fill-rule="evenodd" d="M8.22 1.754a.25.25 0 00-.44 0L1.698 13.132a.25.25 0 00.22.368h12.164a.25.25 0 00.22-.368L8.22 1.754zm-1.763-.707c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0114.082 15H1.918a1.75 1.75 0 01-1.543-2.575L6.457 1.047zM9 11a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.25a.75.75 0 00-1.5 0v2.5a.75.75 0 001.5 0v-2.5z"></path>
</svg>

      <div class="overflow-hidden">This commit does not belong to any branch on this repository, and may belong to a fork outside of the repository.</div>


  
</div></div>

    <include-fragment src="/sean207cc/AI-course/spoofed_commit_check/40389cfbf5b975c899afa75d854d60d2d9e4c7c5" data-test-selector="spoofed-commit-check"></include-fragment>

    <div class="Box d-flex flex-column flex-shrink-0 mb-3">
  <include-fragment src="/sean207cc/AI-course/contributors/gh-pages/_posts/2022-12-08-Pose-Estimation.md" class="commit-loader">
    <div class="Box-header d-flex flex-items-center">
      <div class="Skeleton avatar avatar-user flex-shrink-0 ml-n1 mr-n1 mt-n1 mb-n1" style="width:24px;height:24px;"></div>
      <div class="Skeleton Skeleton--text col-5 ml-2">&nbsp;</div>
    </div>

    <div class="Box-body d-flex flex-items-center" >
      <div class="Skeleton Skeleton--text col-1">&nbsp;</div>
      <span class="color-fg-danger h6 loader-error">Cannot retrieve contributors at this time</span>
    </div>
</include-fragment></div>



      








    <readme-toc>

    <div data-target="readme-toc.content" class="Box mt-3 position-relative">
      
  <div
    class="Box-header js-blob-header blob-header js-sticky js-position-sticky top-0 p-2 d-flex flex-shrink-0 flex-md-row flex-items-center"
    style="position: sticky; z-index: 1;"
  >

      <details
  data-target="readme-toc.trigger"
  data-menu-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;trigger&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}"
  data-menu-hydro-click-hmac="baae4b5c70734451b4a6c99717aa0e79319111065af94aa303ed69442141258f"
  class="dropdown details-reset details-overlay"
>
  <summary
    class="btn btn-octicon m-0 mr-2 p-2"
    aria-haspopup="true"
    aria-label="Table of Contents">
    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-list-unordered">
    <path fill-rule="evenodd" d="M2 4a1 1 0 100-2 1 1 0 000 2zm3.75-1.5a.75.75 0 000 1.5h8.5a.75.75 0 000-1.5h-8.5zm0 5a.75.75 0 000 1.5h8.5a.75.75 0 000-1.5h-8.5zm0 5a.75.75 0 000 1.5h8.5a.75.75 0 000-1.5h-8.5zM3 8a1 1 0 11-2 0 1 1 0 012 0zm-1 6a1 1 0 100-2 1 1 0 000 2z"></path>
</svg>
  </summary>


  <details-menu class="SelectMenu" role="menu">
    <div class="SelectMenu-modal rounded-3 mt-1" style="max-height:340px;">

        <div class="SelectMenu-filter">
          <input
            class="SelectMenu-input form-control js-filterable-field"
            id="toc-filter-field"
            type="text"
            autocomplete="off"
            spellcheck="false"
            autofocus
            placeholder="Filter headings"
            aria-label="Filter headings">
        </div>

      <div class="SelectMenu-list SelectMenu-list--borderless p-2" style="overscroll-behavior: contain;" data-filterable-for="toc-filter-field" data-filterable-type="substring">
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#pose-estimation-applications">Pose Estimation Applications</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 24px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#body-pose">Body Pose</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#bodypix---person-segmentation-in-the-browser">BodyPix - Person Segmentation in the Browser</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#openpose">OpenPose</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#posenet">PoseNet</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#pose-recognition">Pose Recognition</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#mmpose">MMPose</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#densepose-rcnn">DensePose RCNN</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#multi-person-part-segmentation">Multi-Person Part Segmentation</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 24px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#head-pose">Head Pose</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#head-pose-estimation">Head Pose Estimation</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#hopenet">Hopenet</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 24px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#vtuber">VTuber</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#vtuber-unity--head-pose-estimation-face-alignment-gazetracking">VTuber-Unity = Head-Pose-Estimation + Face-Alignment + GazeTracking**</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#vroid-studio">VRoid Studio</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#vtuber_unity">VTuber_Unity</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#openvtuber">OpenVtuber</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 24px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#hand-pose">Hand Pose</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#hand3d">Hand3D</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#deehps">DeeHPS</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#graphposegan">GraphPoseGAN</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#3d-hand-shape">3D Hand Shape</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#facebook-interhand26m">FaceBook InterHand2.6M</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#frankmocap-fast-monocular-3d-hand-and-body-motion-capture-by-regression-and-integration">FrankMocap: Fast Monocular 3D Hand and Body Motion Capture by Regression and Integration</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#a-skeleton-driven-neural-occupancy-representation-for-articulated-hands">A Skeleton-Driven Neural Occupancy Representation for Articulated Hands</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#towards-unconstrained-joint-hand-object-reconstruction-from-rgb-videos">Towards unconstrained joint hand-object reconstruction from RGB videos</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#fast-monocular-hand-pose-estimation-on-embedded-systems">Fast Monocular Hand Pose Estimation on Embedded Systems</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#recent-advances-in-3d-object-and-hand-pose-estimation">Recent Advances in 3D Object and Hand Pose Estimation</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 24px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#object-pose">Object Pose</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#benchmark-for-6d-object-pose-">Benchmark for 6D Object Pose </a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#real-time-seamless-single-shot-6d-object-pose-prediction-yolo-6d">Real-Time Seamless Single Shot 6D Object Pose Prediction (YOLO-6D)</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#posecnn">PoseCNN</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#deepim">DeepIM</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#segmentation-driven-pose">Segmentation-driven Pose</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#dpod">DPOD</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#ho-3d_v3-dataset">HO-3D_v3 Dataset</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 24px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#exercises-of-pose-estimation">Exercises of Pose Estimation</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#bodypix">BodyPix</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#posenet-1">PoseNet</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#mmpose-1">MMPose</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 48px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#2d-human-pose">2D Human Pose</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 48px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#2d-human-whole-body">2D Human Whole-Body</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 48px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#2d-hand-pose">2D Hand Pose</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 48px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#2d-face-keypoints">2D Face Keypoints</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 48px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#3d-human-pose">3D Human Pose</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 48px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#2d-pose-tracking">2D Pose Tracking</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 48px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#2d-animal-pose">2D Animal Pose</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 48px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#3d-hand-pose">3D Hand Pose</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 48px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#webcam-effect">WebCam Effect</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#openpose-1">OpenPose</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#pose-recognition-姿態辨識">Pose Recognition (姿態辨識)</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#head-pose-estimation-1">Head Pose Estimation</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#vtuber-unity">VTuber-Unity</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#openvtuber-1">OpenVtuber</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="afd1519fc6c749e5525faf45709fb8711b2539a4978f27c41db634f22781d8a9" href="#hand-pose-1">Hand Pose</a>
      </div>
    </div>
  </details-menu>
</details>


  <div class="text-mono f6 flex-auto pr-3 flex-order-2 flex-md-order-1">

      454 lines (357 sloc)
      <span class="file-info-divider"></span>
    23 KB
  </div>

  <div class="d-flex py-1 py-md-0 flex-auto flex-order-1 flex-md-order-2 flex-sm-grow-0 flex-justify-between hide-sm hide-md">
        <div class="BtnGroup">
      <a href="/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md?plain=1" data-permalink-href="/sean207cc/AI-course/blob/40389cfbf5b975c899afa75d854d60d2d9e4c7c5/_posts/2022-12-08-Pose-Estimation.md?plain=1" aria-label="Display the source blob" data-view-component="true" class="source tooltipped tooltipped tooltipped-n  js-permalink-replaceable-link btn-sm btn BtnGroup-item">    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-code">
    <path fill-rule="evenodd" d="M4.72 3.22a.75.75 0 011.06 1.06L2.06 8l3.72 3.72a.75.75 0 11-1.06 1.06L.47 8.53a.75.75 0 010-1.06l4.25-4.25zm6.56 0a.75.75 0 10-1.06 1.06L13.94 8l-3.72 3.72a.75.75 0 101.06 1.06l4.25-4.25a.75.75 0 000-1.06l-4.25-4.25z"></path>
</svg>
</a>      <a href="/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md" data-permalink-href="/sean207cc/AI-course/blob/40389cfbf5b975c899afa75d854d60d2d9e4c7c5/_posts/2022-12-08-Pose-Estimation.md" aria-label="Display the rendered blob" data-view-component="true" class="rendered tooltipped tooltipped tooltipped-n selected js-permalink-replaceable-link btn-sm btn BtnGroup-item">    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-file">
    <path fill-rule="evenodd" d="M3.75 1.5a.25.25 0 00-.25.25v12.5c0 .138.112.25.25.25h9.5a.25.25 0 00.25-.25V6h-2.75A1.75 1.75 0 019 4.25V1.5H3.75zm6.75.062V4.25c0 .138.112.25.25.25h2.688a.252.252 0 00-.011-.013l-2.914-2.914a.272.272 0 00-.013-.011zM2 1.75C2 .784 2.784 0 3.75 0h6.586c.464 0 .909.184 1.237.513l2.914 2.914c.329.328.513.773.513 1.237v9.586A1.75 1.75 0 0113.25 16h-9.5A1.75 1.75 0 012 14.25V1.75z"></path>
</svg>
</a>  </div>


    <div class="BtnGroup">
        <a data-permalink-href="/sean207cc/AI-course/raw/40389cfbf5b975c899afa75d854d60d2d9e4c7c5/_posts/2022-12-08-Pose-Estimation.md" href="/sean207cc/AI-course/raw/gh-pages/_posts/2022-12-08-Pose-Estimation.md" id="raw-url" data-view-component="true" class="js-permalink-replaceable-link btn-sm btn BtnGroup-item">    Raw
</a>          <a data-permalink-href="/sean207cc/AI-course/blame/40389cfbf5b975c899afa75d854d60d2d9e4c7c5/_posts/2022-12-08-Pose-Estimation.md" href="/sean207cc/AI-course/blame/gh-pages/_posts/2022-12-08-Pose-Estimation.md" data-hotkey="b" data-view-component="true" class="js-update-url-with-hash js-permalink-replaceable-link btn-sm btn BtnGroup-item">    Blame
</a>    </div>

    <div class="d-flex">
        
<div class="ml-1" data-test-selector="edit-dropdown-menu-component">
  <form class="BtnGroup-parent js-update-url-with-hash " data-turbo="false" action="/sean207cc/AI-course/edit/gh-pages/_posts/2022-12-08-Pose-Estimation.md" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="mfJMeLK34l5S_-k613g1u5jRuyt9CheCWpx8UGPBCGczJ3ZPX-wFsTb5NWd2kZnDHb5Zf57VZmdbcrJP0iTETA" autocomplete="off" />
      <button title="Edit this file" data-hotkey="e" data-disable-with="" data-test-selector="edit-icon-button" type="submit" data-view-component="true" class="btn-sm BtnGroup-item btn">    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-pencil">
    <path fill-rule="evenodd" d="M11.013 1.427a1.75 1.75 0 012.474 0l1.086 1.086a1.75 1.75 0 010 2.474l-8.61 8.61c-.21.21-.47.364-.756.445l-3.251.93a.75.75 0 01-.927-.928l.929-3.25a1.75 1.75 0 01.445-.758l8.61-8.61zm1.414 1.06a.25.25 0 00-.354 0L10.811 3.75l1.439 1.44 1.263-1.263a.25.25 0 000-.354l-1.086-1.086zM11.189 6.25L9.75 4.81l-6.286 6.287a.25.25 0 00-.064.108l-.558 1.953 1.953-.558a.249.249 0 00.108-.064l6.286-6.286z"></path>
</svg>
</button></form>
  <details class="details-reset details-overlay select-menu BtnGroup-parent d-inline-block position-relative">
      <summary data-disable-invalid="" data-disable-with="" data-dropdown-tracking="{&quot;type&quot;:&quot;blob_edit_dropdown.more_options_click&quot;,&quot;context&quot;:{&quot;repository_id&quot;:575813281,&quot;actor_id&quot;:114159512,&quot;github_dev_enabled&quot;:true,&quot;edit_enabled&quot;:true,&quot;small_screen&quot;:false}}" aria-label="Select additional options" data-view-component="true" class="js-blob-dropdown-click select-menu-button btn-sm btn BtnGroup-item float-none px-2">
</summary>    <div class="SelectMenu right-0">
      <div class="SelectMenu-modal width-full">
        <div class="SelectMenu-list SelectMenu-list--borderless py-2">
          <form class="SelectMenu-item js-update-url-with-hash " data-turbo="false" action="/sean207cc/AI-course/edit/gh-pages/_posts/2022-12-08-Pose-Estimation.md" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="2BUYVyaOHgaobD5OOrqZyFJb_gYE_jByWa8dQQrIUhBywCJgy9X56cxq4hObUzWw1zQcUuchQZdYQdNeuy2eOw" autocomplete="off" />
              <button title="Edit this file" data-test-selector="edit-text-button" type="submit" data-view-component="true" class="btn-invisible btn width-full d-flex flex-justify-between color-fg-default text-normal p-0">    <div class="mr-5">Edit this file</div>
              <div class="color-fg-muted">E</div>
</button></form>
            <a aria-label="Open this file in github.dev" data-test-selector="github-dev-link" data-dropdown-tracking="{&quot;type&quot;:&quot;blob_edit_dropdown.dev_link_click&quot;,&quot;context&quot;:{&quot;repository_id&quot;:575813281,&quot;actor_id&quot;:114159512,&quot;edit_enabled&quot;:true,&quot;small_screen&quot;:false}}" href="https://github.dev/" data-view-component="true" class="SelectMenu-item js-github-dev-shortcut js-blob-dropdown-click width-full d-flex flex-justify-between color-fg-default f5 text-normal">
              <div class="mr-5 no-wrap">Open in github.dev</div>
              <div class="color-fg-muted">.</div>
</a>
            <a data-platforms="windows,mac" data-test-selector="github-desktop-link" aria-label="Open this file in GitHub Desktop" href="https://desktop.github.com" data-view-component="true" class="SelectMenu-item no-wrap js-remove-unless-platform width-full text-normal color-fg-default f5">
              Open in GitHub Desktop
</a>        </div>
      </div>
    </div>
  </details>
</div>


        
<div data-test-selector="remote-clipboard-copy">
  <remote-clipboard-copy class="d-inline-block btn-octicon" style="height: 26px" data-src="/sean207cc/AI-course/raw/40389cfbf5b975c899afa75d854d60d2d9e4c7c5/_posts/2022-12-08-Pose-Estimation.md" data-action="click:remote-clipboard-copy#remoteCopy">
  

  <span data-target="remote-clipboard-copy.idle">      <span class="tooltipped tooltipped-nw cursor-pointer" data-hydro-click="{&quot;event_type&quot;:&quot;repository.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;COPY_RAW_CONTENTS_BUTTON&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="5ac1ff50a8ec54848f9b1ab4ac58835140a516b00c6366c87fbd6247d511fe79" aria-label="Copy raw contents">
        <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy">
    <path fill-rule="evenodd" d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 010 1.5h-1.5a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-1.5a.75.75 0 011.5 0v1.5A1.75 1.75 0 019.25 16h-7.5A1.75 1.75 0 010 14.25v-7.5z"></path><path fill-rule="evenodd" d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0114.25 11h-7.5A1.75 1.75 0 015 9.25v-7.5zm1.75-.25a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-7.5a.25.25 0 00-.25-.25h-7.5z"></path>
</svg>
</span></span>
  <span data-target="remote-clipboard-copy.fetching" hidden="hidden">      <svg style="box-sizing: content-box; color: var(--color-icon-primary);" width="16" height="16" viewBox="0 0 16 16" fill="none" data-view-component="true" class="anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" />
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke" />
</svg>
</span>
  <span data-target="remote-clipboard-copy.success" hidden="hidden">      <span class="tooltipped tooltipped-nw" aria-label="Copied!">
        <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check color-fg-success">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
      </span>
</span>
  <span data-target="remote-clipboard-copy.error" hidden="hidden">      <span class="tooltipped tooltipped-nw" aria-label="Something went wrong. Try again.">
        <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-alert color-fg-attention">
    <path fill-rule="evenodd" d="M8.22 1.754a.25.25 0 00-.44 0L1.698 13.132a.25.25 0 00.22.368h12.164a.25.25 0 00.22-.368L8.22 1.754zm-1.763-.707c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0114.082 15H1.918a1.75 1.75 0 01-1.543-2.575L6.457 1.047zM9 11a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.25a.75.75 0 00-1.5 0v2.5a.75.75 0 001.5 0v-2.5z"></path>
</svg>
      </span>
</span>
</remote-clipboard-copy></div>


          <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="inline-form" data-turbo="false" action="/sean207cc/AI-course/delete/gh-pages/_posts/2022-12-08-Pose-Estimation.md" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="mzs_vFhm6UUN-iYT1u7x-cx-ZxfXp-q73bdXRtx2hdmyPYtZlfJLZR9rUP7Srry4e8wrS3Vht5yoHHmLYDQMgQ" />
            <button class="btn-octicon btn-octicon-danger tooltipped tooltipped-nw" type="submit"
              aria-label="Delete this file" data-disable-with>
              <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-trash">
    <path fill-rule="evenodd" d="M6.5 1.75a.25.25 0 01.25-.25h2.5a.25.25 0 01.25.25V3h-3V1.75zm4.5 0V3h2.25a.75.75 0 010 1.5H2.75a.75.75 0 010-1.5H5V1.75C5 .784 5.784 0 6.75 0h2.5C10.216 0 11 .784 11 1.75zM4.496 6.675a.75.75 0 10-1.492.15l.66 6.6A1.75 1.75 0 005.405 15h5.19c.9 0 1.652-.681 1.741-1.576l.66-6.6a.75.75 0 00-1.492-.149l-.66 6.6a.25.25 0 01-.249.225h-5.19a.25.25 0 01-.249-.225l-.66-6.6z"></path>
</svg>
            </button>
</form>    </div>
  </div>

    <div class="d-flex hide-lg hide-xl flex-order-2 flex-grow-0">
      <details class="dropdown details-reset details-overlay d-inline-block">
        <summary
          class="js-blob-dropdown-click btn-octicon p-2"
          aria-haspopup="true"
          aria-label="possible actions"
          data-test-selector="small-screen-more-options"
          data-dropdown-tracking="{&quot;type&quot;:&quot;blob_edit_dropdown.more_options_click&quot;,&quot;context&quot;:{&quot;repository_id&quot;:575813281,&quot;actor_id&quot;:114159512,&quot;github_dev_enabled&quot;:true,&quot;edit_enabled&quot;:true,&quot;small_screen&quot;:true}}"
        >
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-kebab-horizontal">
    <path d="M8 9a1.5 1.5 0 100-3 1.5 1.5 0 000 3zM1.5 9a1.5 1.5 0 100-3 1.5 1.5 0 000 3zm13 0a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path>
</svg>
        </summary>

        <ul class="dropdown-menu dropdown-menu-sw" style="width: 175px">
            <li>
                <a class="dropdown-item tooltipped tooltipped-nw js-remove-unless-platform"
                   data-platforms="windows,mac"
                   href="https://desktop.github.com">
                  Open with Desktop
                </a>
            </li>
          <li>
            <a class="dropdown-item" href="/sean207cc/AI-course/raw/gh-pages/_posts/2022-12-08-Pose-Estimation.md">
              View raw
            </a>
          </li>
            <li>
              <remote-clipboard-copy class="dropdown-item" data-src="/sean207cc/AI-course/raw/gh-pages/_posts/2022-12-08-Pose-Estimation.md" data-action="click:remote-clipboard-copy#remoteCopy">
  

  <span data-target="remote-clipboard-copy.idle">                  <span class="cursor-pointer" data-hydro-click="{&quot;event_type&quot;:&quot;repository.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;COPY_RAW_CONTENTS_BUTTON&quot;,&quot;repository_id&quot;:575813281,&quot;originating_url&quot;:&quot;https://github.com/sean207cc/AI-course/blob/gh-pages/_posts/2022-12-08-Pose-Estimation.md&quot;,&quot;user_id&quot;:114159512}}" data-hydro-click-hmac="5ac1ff50a8ec54848f9b1ab4ac58835140a516b00c6366c87fbd6247d511fe79">
                    Copy raw contents
</span></span>
  <span data-target="remote-clipboard-copy.fetching" hidden="hidden">                  Copy raw contents
                  <span class="d-inline-block position-relative" style="top: 3px">
                    <svg aria-label="fetching contents…" style="box-sizing: content-box; color: var(--color-icon-primary);" width="16" height="16" viewBox="0 0 16 16" fill="none" data-view-component="true" class="anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" />
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke" />
</svg>
                  </span>
</span>
  <span data-target="remote-clipboard-copy.success" hidden="hidden">                  Copy raw contents
                  <svg aria-label="Copied!" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check color-fg-success">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
</span>
  <span data-target="remote-clipboard-copy.error" hidden="hidden">                  Copy raw contents
                  <svg aria-label="Something went wrong. Try again." role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-alert color-fg-attention">
    <path fill-rule="evenodd" d="M8.22 1.754a.25.25 0 00-.44 0L1.698 13.132a.25.25 0 00.22.368h12.164a.25.25 0 00.22-.368L8.22 1.754zm-1.763-.707c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0114.082 15H1.918a1.75 1.75 0 01-1.543-2.575L6.457 1.047zM9 11a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.25a.75.75 0 00-1.5 0v2.5a.75.75 0 001.5 0v-2.5z"></path>
</svg>
</span>
</remote-clipboard-copy>            </li>
            <li>
              <a class="dropdown-item" href="/sean207cc/AI-course/blame/gh-pages/_posts/2022-12-08-Pose-Estimation.md">
                View blame
              </a>
            </li>

              <li class="dropdown-divider" role="none"></li>
              <li>
                <a class="dropdown-item" href="/sean207cc/AI-course/edit/gh-pages/_posts/2022-12-08-Pose-Estimation.md">Edit file</a>
              </li>
                <li>
                  <a class="dropdown-item js-github-dev-shortcut js-blob-dropdown-click" data-test-selector="small-screen-github-dev-link" data-dropdown-tracking="{&quot;type&quot;:&quot;blob_edit_dropdown.dev_link_click&quot;,&quot;context&quot;:{&quot;repository_id&quot;:575813281,&quot;actor_id&quot;:114159512,&quot;edit_enabled&quot;:true,&quot;small_screen&quot;:true}}" href="https://github.dev/">Open with github.dev</a>
                </li>
              <li>
                <a class="dropdown-item menu-item-danger" href="/sean207cc/AI-course/delete/gh-pages/_posts/2022-12-08-Pose-Estimation.md">Delete file</a>
              </li>
        </ul>
      </details>
    </div>
</div>


        <div id="readme" class="Box-body readme blob js-code-block-container p-5 p-xl-6 gist-border-0">
    <article class="markdown-body entry-content container-lg" itemprop="text"><table>
  <thead>
  <tr>
  <th>layout</th>
  <th>title</th>
  <th>author</th>
  <th>category</th>
  <th>tags</th>
  </tr>
  </thead>
  <tbody>
  <tr>
  <td><div dir="auto">post</div></td>
  <td><div dir="auto">Pose Estimation</div></td>
  <td><div dir="auto"><table>
  <tbody>
  <tr>
  <td><div dir="auto">Richard Kuo</div></td>
  </tr>
  </tbody>
</table>
</div></td>
  <td><div dir="auto"><table>
  <tbody>
  <tr>
  <td><div dir="auto">Lecture</div></td>
  </tr>
  </tbody>
</table>
</div></td>
  <td><div dir="auto"><table>
  <tbody>
  <tr>
  <td><div dir="auto">jekyll</div></td>
  <td><div dir="auto">ai</div></td>
  </tr>
  </tbody>
</table>
</div></td>
  </tr>
  </tbody>
</table>

<p dir="auto">Pose Estimation includes Applications, Body Pose, Head Pose, Hand Pose , Object Pose.</p>
<hr>
<h3 dir="auto"><a id="user-content-pose-estimation-applications" class="anchor" aria-hidden="true" href="#pose-estimation-applications"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Pose Estimation Applications</h3>
<ul dir="auto">
<li>
<p dir="auto"><strong><a href="https://johnsonfitnesslive.com/?action=mirror_pro_intro" rel="nofollow">健身鏡</a></strong><br>
<a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/64805216badf6c035ee534a2899eb65a0386ea40f677bbe2bd958cc2447dec2c/68747470733a2f2f6a6f686e736f6e6669746e6573736c6976652e636f6d2f696d616765732f6d6972726f7250726f2d706172616c6c61782d6267322d696d6730332e676966"><img src="https://camo.githubusercontent.com/64805216badf6c035ee534a2899eb65a0386ea40f677bbe2bd958cc2447dec2c/68747470733a2f2f6a6f686e736f6e6669746e6573736c6976652e636f6d2f696d616765732f6d6972726f7250726f2d706172616c6c61782d6267322d696d6730332e676966" alt="" data-animated-image="" data-canonical-src="https://johnsonfitnesslive.com/images/mirrorPro-parallax-bg2-img03.gif" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto"><strong><a href="https://fc.bnext.com.tw/articles/view/1226" rel="nofollow">AI健身教練</a></strong><br>
健身新創 Peloton 在這波居家健身浪潮下，以販售主力產品飛輪、跑步機搭配線上課程，並將健身教練打造成「網紅」，用心拍攝運動影片，成功創造粉絲經濟。<br>
<a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/18210b18937479ae2c828559405254c59aad109d56ada730a2a12a0fc59ffd87/68747470733a2f2f626e6578746d656469612e73332e6869636c6f75642e6e65742e74772f696d6167652f616c62756d2f323032312d30332f696d672d313631343835363334312d3639373733403630302e6a7067"><img src="https://camo.githubusercontent.com/18210b18937479ae2c828559405254c59aad109d56ada730a2a12a0fc59ffd87/68747470733a2f2f626e6578746d656469612e73332e6869636c6f75642e6e65742e74772f696d6167652f616c62756d2f323032312d30332f696d672d313631343835363334312d3639373733403630302e6a7067" alt="" data-canonical-src="https://bnextmedia.s3.hicloud.net.tw/image/album/2021-03/img-1614856341-69773@600.jpg" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto"><strong><a href="https://www.inside.com.tw/article/21711-aigo-interview-aifly" rel="nofollow">馬術治療</a></strong><br>
<a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/967603c5fc53d1aceb23763a7cf5c15908572b4f2b8be1a6a3abd563e5bf4a8a/68747470733a2f2f696e736964652d617373657473312e696e736964652e636f6d2e74772f323032302f31312f6f7a306675396d616c37326b64707466686e7138763739736636376335372e706e673f773d373330266669743d6d617826713d3830"><img src="https://camo.githubusercontent.com/967603c5fc53d1aceb23763a7cf5c15908572b4f2b8be1a6a3abd563e5bf4a8a/68747470733a2f2f696e736964652d617373657473312e696e736964652e636f6d2e74772f323032302f31312f6f7a306675396d616c37326b64707466686e7138763739736636376335372e706e673f773d373330266669743d6d617826713d3830" alt="" data-canonical-src="https://inside-assets1.inside.com.tw/2020/11/oz0fu9mal72kdptfhnq8v79sf67c57.png?w=730&amp;fit=max&amp;q=80" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto"><strong><a href="https://github.com/burningion/dab-and-tpose-controlled-lights">Pose-controlled Lights</a></strong><br>
<a target="_blank" rel="noopener noreferrer" href="https://github.com/burningion/dab-and-tpose-controlled-lights/raw/master/images/dab-tpose.gif?raw=True"><img src="https://github.com/burningion/dab-and-tpose-controlled-lights/raw/master/images/dab-tpose.gif?raw=True" alt="" data-animated-image="" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto"><strong><a href="https://www.chinatimes.com/realtimenews/20201203005307-260418?chdtv" rel="nofollow">跌倒偵測</a></strong></p>
</li>
</ul>
<table>
  <tbody><tr>
  <td><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/5b4b5fd543bbe83ed351e63e7d752d2cab525367613d3a70152d538f1328a7f3/68747470733a2f2f696d616765732e6368696e6174696d65732e636f6d2f6e65777370686f746f2f323032302d31322d30332f313032342f32303230313230333030353439352e6a7067"><img src="https://camo.githubusercontent.com/5b4b5fd543bbe83ed351e63e7d752d2cab525367613d3a70152d538f1328a7f3/68747470733a2f2f696d616765732e6368696e6174696d65732e636f6d2f6e65777370686f746f2f323032302d31322d30332f313032342f32303230313230333030353439352e6a7067" data-canonical-src="https://images.chinatimes.com/newsphoto/2020-12-03/1024/20201203005495.jpg" style="max-width: 100%;"></a></td>  
  <td><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/8f482a0834a762e12f150a985eac05a0a3e3858b9882f640dbb9aaf18af9e363/68747470733a2f2f6d61746368696e672e6f72672e74772f776562736974652f75706c6f6164735f70726f647563742f776562736974655f312f50303030303130303030303034345f345f3132332e6a7067"><img src="https://camo.githubusercontent.com/8f482a0834a762e12f150a985eac05a0a3e3858b9882f640dbb9aaf18af9e363/68747470733a2f2f6d61746368696e672e6f72672e74772f776562736974652f75706c6f6164735f70726f647563742f776562736974655f312f50303030303130303030303034345f345f3132332e6a7067" data-canonical-src="https://matching.org.tw/website/uploads_product/website_1/P0000100000044_4_123.jpg" style="max-width: 100%;"></a></td>
  </tr>
</tbody></table>
<ul dir="auto">
<li>
<p dir="auto"><strong><a href="https://www.inside.com.tw/article/21716-aigo-interview-beseye-alpha" rel="nofollow">產線SOP</a></strong><br>
以雅文塑膠來說，產線作業員的動作僅集中於上半身，以頭部、頸部、肩膀、手臂、手掌的動作為主。Beseye_alpha 針對需求，複製日本大型製造工廠 AI 模型開發的成功案例、及與客戶多次討論需求、實地作業工作站規劃、實際場域測試資料訓練，開發出一個「肢體律動分析」模型，有效達到降低運算量的目標。</p>
</li>
<li>
<p dir="auto"><strong><a href="https://www.eastwestidea.net/index.php/%E6%9D%90%E6%96%99/item/376" rel="nofollow">其他應用</a></strong><br></p>
</li>
</ul>
<hr>
<h2 dir="auto"><a id="user-content-body-pose" class="anchor" aria-hidden="true" href="#body-pose"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Body Pose</h2>
<p dir="auto"><strong>Ref.</strong> <a href="https://heartbeat.comet.ml/a-2019-guide-to-human-pose-estimation-c10b79b64b73#7c7f" rel="nofollow">A 2019 Guide to Huamn Pose Estimatioin</a><br></p>
<h3 dir="auto"><a id="user-content-bodypix---person-segmentation-in-the-browser" class="anchor" aria-hidden="true" href="#bodypix---person-segmentation-in-the-browser"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>BodyPix - Person Segmentation in the Browser</h3>
<p dir="auto"><strong>Code:</strong> <a href="https://github.com/tensorflow/tfjs-models/tree/master/body-pix">tfjs-models/body-pix</a><br>
<code>pip install tf_bodypix</code>
<a href="https://storage.googleapis.com/tfjs-models/demos/body-pix/index.html" rel="nofollow">Live Demo</a></p>
<h2 dir="auto"><a id="" class="anchor" aria-hidden="true" href="#"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><a target="_blank" rel="noopener noreferrer" href="https://github.com/tensorflow/tfjs-models/raw/master/body-pix/images/body-pix-2.0.gif"><img src="https://github.com/tensorflow/tfjs-models/raw/master/body-pix/images/body-pix-2.0.gif" alt="" data-animated-image="" style="max-width: 100%;"></a><br></h2>
<h3 dir="auto"><a id="user-content-openpose" class="anchor" aria-hidden="true" href="#openpose"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>OpenPose</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/1812.08008" rel="nofollow">arxiv.org/abs/1812.08008</a><br>
<strong>Code:</strong> <a href="https://github.com/CMU-Perceptual-Computing-Lab/openpose">CMU-Perceptual-Computing-Lab/openpose</a><br>
<strong>Ref.</strong> <a href="https://viso.ai/deep-learning/openpose/" rel="nofollow">A Guide to OpenPose in 2021</a><br></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/.github/media/pose_face_hands.gif?raw=true"><img src="https://github.com/CMU-Perceptual-Computing-Lab/openpose/raw/master/.github/media/pose_face_hands.gif?raw=true" alt="" data-animated-image="" style="max-width: 100%;"></a>
<a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/0b1d5f169e64239155b7c01fdb8f62082391a3ddb78f4f074bfa420aeabd1aa6/68747470733a2f2f7669736f2e61692f77702d636f6e74656e742f75706c6f6164732f323032312f30312f4b6579706f696e74732d44657465637465642d62792d4f70656e506f73652d6f6e2d7468652d434f434f2d446174617365742e6a7067"><img src="https://camo.githubusercontent.com/0b1d5f169e64239155b7c01fdb8f62082391a3ddb78f4f074bfa420aeabd1aa6/68747470733a2f2f7669736f2e61692f77702d636f6e74656e742f75706c6f6164732f323032312f30312f4b6579706f696e74732d44657465637465642d62792d4f70656e506f73652d6f6e2d7468652d434f434f2d446174617365742e6a7067" alt="" data-canonical-src="https://viso.ai/wp-content/uploads/2021/01/Keypoints-Detected-by-OpenPose-on-the-COCO-Dataset.jpg" style="max-width: 100%;"></a>
<a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/959c388c3760b15fa1a1db3b69e7a78b27c2053fd10ae7d10adc12edd5843232/68747470733a2f2f6d656469612e61727869762d76616e6974792e636f6d2f72656e6465722d6f75747075742f353530393833322f78322e706e67"><img src="https://camo.githubusercontent.com/959c388c3760b15fa1a1db3b69e7a78b27c2053fd10ae7d10adc12edd5843232/68747470733a2f2f6d656469612e61727869762d76616e6974792e636f6d2f72656e6465722d6f75747075742f353530393833322f78322e706e67" alt="" data-canonical-src="https://media.arxiv-vanity.com/render-output/5509832/x2.png" style="max-width: 100%;"></a></p>
&lt;iframe width="960" height="540" src="<a href="https://www.youtube.com/embed/0XIm-NTnOYc" rel="nofollow">https://www.youtube.com/embed/0XIm-NTnOYc</a>" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen&gt;&lt;/iframe&gt;
<hr>
<h3 dir="auto"><a id="user-content-posenet" class="anchor" aria-hidden="true" href="#posenet"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>PoseNet</h3>

PoseNet is built to run on lightweight devices such as the browser or mobile device where as<br>
OpenPose is much more accurate and meant to be ran on GPU powered systems. You can see the performance benchmarks below.<br>

**Paper:**  [arxiv.org/abs/1505.07427](<a href="https://arxiv.org/abs/1505.07427" rel="nofollow">https://arxiv.org/abs/1505.07427</a>)<br>
**Code:** [rwightman/posenet-pytorch](<a href="https://github.com/rwightman/posenet-pytorch">https://github.com/rwightman/posenet-pytorch</a>)<br>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/2da1cc7aa187e04fc949b7a86c46fadffa691e8c3f69e0283687db3b839d9a9b/68747470733a2f2f6465627567676572636166652e636f6d2f77702d636f6e74656e742f75706c6f6164732f323032302f31302f6b6579706f696e745f65786d702e6a7067"><img src="https://camo.githubusercontent.com/2da1cc7aa187e04fc949b7a86c46fadffa691e8c3f69e0283687db3b839d9a9b/68747470733a2f2f6465627567676572636166652e636f6d2f77702d636f6e74656e742f75706c6f6164732f323032302f31302f6b6579706f696e745f65786d702e6a7067" alt="" data-canonical-src="https://debuggercafe.com/wp-content/uploads/2020/10/keypoint_exmp.jpg" style="max-width: 100%;"></a>
<a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/818c73facab68dd8bf7e3e0dec462476dcbb66ee0044c27899e95e1817e5830a/68747470733a2f2f7777772e7265736561726368676174652e6e65742f70726f66696c652f536f726f7573682d53656966692f7075626c69636174696f6e2f3333353938393934352f6669677572652f666967322f41533a38303634393935353532333337393340313536393239353838363934362f5468652d506f73656e65742d6172636869746563747572652d59656c6c6f772d6d6f64756c65732d6172652d7368617265642d776974682d476f6f676c654e65742d7768696c652d677265656e2d6d6f64756c65732e70706d"><img src="https://camo.githubusercontent.com/818c73facab68dd8bf7e3e0dec462476dcbb66ee0044c27899e95e1817e5830a/68747470733a2f2f7777772e7265736561726368676174652e6e65742f70726f66696c652f536f726f7573682d53656966692f7075626c69636174696f6e2f3333353938393934352f6669677572652f666967322f41533a38303634393935353532333337393340313536393239353838363934362f5468652d506f73656e65742d6172636869746563747572652d59656c6c6f772d6d6f64756c65732d6172652d7368617265642d776974682d476f6f676c654e65742d7768696c652d677265656e2d6d6f64756c65732e70706d" alt="" data-canonical-src="https://www.researchgate.net/profile/Soroush-Seifi/publication/335989945/figure/fig2/AS:806499555233793@1569295886946/The-Posenet-architecture-Yellow-modules-are-shared-with-GoogleNet-while-green-modules.ppm" style="max-width: 100%;"></a>
<a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/0c249eade4836c4f94f5218c39b0d4960871e4f594368465277b19845719fbd4/68747470733a2f2f69312e77702e636f6d2f7061726c65796c6162732e636f6d2f77702d636f6e74656e742f75706c6f6164732f323032302f30312f696d6167652d312e706e673f726573697a653d313032342532433432302673736c3d31"><img src="https://camo.githubusercontent.com/0c249eade4836c4f94f5218c39b0d4960871e4f594368465277b19845719fbd4/68747470733a2f2f69312e77702e636f6d2f7061726c65796c6162732e636f6d2f77702d636f6e74656e742f75706c6f6164732f323032302f30312f696d6167652d312e706e673f726573697a653d313032342532433432302673736c3d31" alt="" data-canonical-src="https://i1.wp.com/parleylabs.com/wp-content/uploads/2020/01/image-1.png?resize=1024%2C420&amp;ssl=1" style="max-width: 100%;"></a></p>
<hr>
<h3 dir="auto"><a id="user-content-pose-recognition" class="anchor" aria-hidden="true" href="#pose-recognition"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Pose Recognition</h3>
<p dir="auto"><em>using Pose keypoints as dataset to train a DNN</em><br>
<strong>Code:</strong> <a href="https://github.com/burningion/dab-and-tpose-controlled-lights">burningion/dab-and-tpose-controlled-lights</a><br>
<strong>IPYNB:</strong> <a href="https://github.com/burningion/dab-and-tpose-controlled-lights/blob/master/Data%20Play.ipynb">pose-control-lights</a><br></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/burningion/dab-and-tpose-controlled-lights/raw/master/images/dab-tpose.gif"><img src="https://github.com/burningion/dab-and-tpose-controlled-lights/raw/master/images/dab-tpose.gif" alt="" data-animated-image="" style="max-width: 100%;"></a>
<a target="_blank" rel="noopener noreferrer nofollow" href="https://raw.githubusercontent.com/burningion/dab-and-tpose-controlled-lights/master/images/neural1.png"><img src="https://raw.githubusercontent.com/burningion/dab-and-tpose-controlled-lights/master/images/neural1.png" alt="" style="max-width: 100%;"></a></p>
<hr>
<h3 dir="auto"><a id="user-content-mmpose" class="anchor" aria-hidden="true" href="#mmpose"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>MMPose</h3>
<p dir="auto"><strong>Code:</strong> <a href="https://github.com/open-mmlab/mmpose">open-mmlab</a><br>
<strong><a href="https://github.com/open-mmlab/mmpose#model-zoo">Model Zoo</a></strong> <br></p>
&lt;iframe width="920" height="520" src="<a href="https://user-images.githubusercontent.com/15977946/124654387-0fd3c500-ded1-11eb-84f6-24eeddbf4d91.mp4" rel="nofollow">https://user-images.githubusercontent.com/15977946/124654387-0fd3c500-ded1-11eb-84f6-24eeddbf4d91.mp4</a>" title="MMPos Demo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen&gt;&lt;/iframe&gt;
<hr>
<h3 dir="auto"><a id="user-content-densepose-rcnn" class="anchor" aria-hidden="true" href="#densepose-rcnn"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>DensePose RCNN</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/1802.00434" rel="nofollow">arxiv.org/abs/1802.00434</a><br>
<strong>Code:</strong> <a href="https://github.com/facebookresearch/Densepose">facebookresearch/DensePose</a><br></p>
<p align="center" dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/be4698fcd4b3b976b2ec5ebd489e91c1b206c8ef350e46031c05071311d1fe6c/68747470733a2f2f646c2e666261697075626c696366696c65732e636f6d2f64656e7365706f73652f7765622f64656e7365706f73655f7465617365725f636f6d707265737365645f32352e676966"><img src="https://camo.githubusercontent.com/be4698fcd4b3b976b2ec5ebd489e91c1b206c8ef350e46031c05071311d1fe6c/68747470733a2f2f646c2e666261697075626c696366696c65732e636f6d2f64656e7365706f73652f7765622f64656e7365706f73655f7465617365725f636f6d707265737365645f32352e676966" style="max-width: 100%;"></a></p>
<p dir="auto"><strong>Region-based DensePose architecture</strong><br></p>
<p align="center" dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/cf1309bec63183a3882a1aac7c66b44038fef16e511cdfaee5743ea11ec540bb/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f3730302f312a6934474c7933464e6c3753536c326a337549386d56672e706e67"><img src="https://camo.githubusercontent.com/cf1309bec63183a3882a1aac7c66b44038fef16e511cdfaee5743ea11ec540bb/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f3730302f312a6934474c7933464e6c3753536c326a337549386d56672e706e67" data-canonical-src="https://miro.medium.com/max/700/1*i4GLy3FNl7SSl2j3uI8mVg.png" style="max-width: 100%;"></a></p>
<p dir="auto"><strong>Multi-task cascaded architectures</strong><br></p>
<p align="center" dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/87321bc78fe8445c90ccac79e6fb11fece8a21d764703aa34112df6668b9ce90/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f3730302f312a464b4a5250676d3752555a646e76647154544d6538672e706e67"><img src="https://camo.githubusercontent.com/87321bc78fe8445c90ccac79e6fb11fece8a21d764703aa34112df6668b9ce90/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f3730302f312a464b4a5250676d3752555a646e76647154544d6538672e706e67" data-canonical-src="https://miro.medium.com/max/700/1*FKJRPgm7RUZdnvdqTTMe8g.png" style="max-width: 100%;"></a></p>
<hr>
<h3 dir="auto"><a id="user-content-multi-person-part-segmentation" class="anchor" aria-hidden="true" href="#multi-person-part-segmentation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Multi-Person Part Segmentation</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/1907.05193" rel="nofollow">arxiv.org/abs/1907.05193</a><br>
<strong>Code:</strong> <a href="https://github.com/kevinlin311tw/CDCL-human-part-segmentation">kevinlin311tw/CDCL-human-part-segmentation</a></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/kevinlin311tw/CDCL-human-part-segmentation/blob/master/cdcl_teaser.jpg?raw=true"><img src="https://github.com/kevinlin311tw/CDCL-human-part-segmentation/raw/master/cdcl_teaser.jpg?raw=true" alt="" style="max-width: 100%;"></a></p>
<hr>
<h2 dir="auto"><a id="user-content-head-pose" class="anchor" aria-hidden="true" href="#head-pose"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Head Pose</h2>
<h3 dir="auto"><a id="user-content-head-pose-estimation" class="anchor" aria-hidden="true" href="#head-pose-estimation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Head Pose Estimation</h3>
<p dir="auto"><strong>Code:</strong><a href="https://github.com/yinguobing/head-pose-estimation">yinguobing/head-pose-estimation</a><br></p>
<table>
  <tbody><tr>
    <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/rkuo2000/head-pose-estimation/blob/master/doc/demo.gif?raw=true"><img src="https://github.com/rkuo2000/head-pose-estimation/raw/master/doc/demo.gif?raw=true" data-animated-image="" style="max-width: 100%;"></a></td>
    <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/rkuo2000/head-pose-estimation/blob/master/doc/demo1.gif?raw=true"><img src="https://github.com/rkuo2000/head-pose-estimation/raw/master/doc/demo1.gif?raw=true" data-animated-image="" style="max-width: 100%;"></a></td>
  </tr>
</tbody></table>
<h3 dir="auto"><a id="user-content-hopenet" class="anchor" aria-hidden="true" href="#hopenet"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Hopenet</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/1710.00925" rel="nofollow">Fine-Grained Head Pose Estimation Without Keypoints</a><br>
<a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/eec1eda5d88c107abf6769b09ebc8cf2e3459bd89b2fa4c7d09c3208bef2aec9/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f3730302f312a4b4665533059597a414f4d3158466f6b476633625a412e706e67"><img src="https://camo.githubusercontent.com/eec1eda5d88c107abf6769b09ebc8cf2e3459bd89b2fa4c7d09c3208bef2aec9/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f3730302f312a4b4665533059597a414f4d3158466f6b476633625a412e706e67" alt="" data-canonical-src="https://miro.medium.com/max/700/1*KFeS0YYzAOM1XFokGf3bZA.png" style="max-width: 100%;"></a></p>
<p dir="auto"><strong>Code:</strong> <a href="https://github.com/natanielruiz/deep-head-pose">deep-head-pose</a><br>
<a target="_blank" rel="noopener noreferrer" href="https://github.com/natanielruiz/deep-head-pose/blob/master/conan-cruise.gif?raw=true"><img src="https://github.com/natanielruiz/deep-head-pose/raw/master/conan-cruise.gif?raw=true" alt="" data-animated-image="" style="max-width: 100%;"></a></p>
<p dir="auto"><strong>Code:</strong> <a href="https://github.com/axinc-ai/ailia-models/tree/master/face_recognition/hopenet">hopenet</a><br>
<strong>Blog:</strong> <a href="https://medium.com/axinc-ai/hope-net-a-machine-learning-model-for-estimating-face-orientation-83d5af26a513" rel="nofollow">HOPE-Net : A Machine Learning Model for Estimating Face Orientation</a></p>
&lt;iframe width="665" height="382" src="<a href="https://www.youtube.com/embed/DA1SACACK0k" rel="nofollow">https://www.youtube.com/embed/DA1SACACK0k</a>" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen&gt;&lt;/iframe&gt;
<hr>
<h2 dir="auto"><a id="user-content-vtuber" class="anchor" aria-hidden="true" href="#vtuber"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>VTuber</h2>
<p dir="auto"><a href="https://www.4gamers.com.tw/news/detail/50500/virtual-youtuber-surpasses-16000" rel="nofollow">Vtuber總數突破16000人，增速不緩一年增加3000人</a>
依據日本數據調查分析公司 User Local 的報告，在該社最新的 <a href="https://virtual-youtuber.userlocal.jp/document/ranking" rel="nofollow">User Local VTuber</a> 排行榜上，有紀錄的 Vtuber 正式突破了 16,000 人。</p>
<p dir="auto">1位 <a href="https://virtual-youtuber.userlocal.jp/user/0DCB37A5BB880687_c8ea33" rel="nofollow">Gawr Gura(がうるぐら サメちゃん)</a> Gawr Gura Ch. hololive-EN</p>
&lt;iframe width="730" height="411" src="<a href="https://www.youtube.com/embed/Hq9BBxGqyCY" rel="nofollow">https://www.youtube.com/embed/Hq9BBxGqyCY</a>" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen&gt;&lt;/iframe&gt;
<p dir="auto">2位 <a href="https://virtual-youtuber.userlocal.jp/user/D780B63C2DEBA9A2_fa95ae" rel="nofollow">キズナアイ</a> A.I.Channel</p>
&lt;iframe width="730" height="411" src="<a href="https://www.youtube.com/embed/ZedmVzmAf3M" rel="nofollow">https://www.youtube.com/embed/ZedmVzmAf3M</a>" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen&gt;&lt;/iframe&gt;
<p dir="auto">3位 <a href="https://virtual-youtuber.userlocal.jp/user/CE32A8A748265090_585651" rel="nofollow">Mori Calliope(森カリオペ)</a> Mori Calliope Ch.</p>
&lt;iframe width="730" height="411" src="<a href="https://www.youtube.com/embed/j-QtsaCscyI" rel="nofollow">https://www.youtube.com/embed/j-QtsaCscyI</a>" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen&gt;&lt;/iframe&gt;
<h3 dir="auto"><a id="user-content-vtuber-unity--head-pose-estimation-face-alignment-gazetracking" class="anchor" aria-hidden="true" href="#vtuber-unity--head-pose-estimation-face-alignment-gazetracking"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>VTuber-Unity = Head-Pose-Estimation + Face-Alignment + GazeTracking**<br></h3>
<h3 dir="auto"><a id="user-content-vroid-studio" class="anchor" aria-hidden="true" href="#vroid-studio"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><a href="https://vroid.com/studio" rel="nofollow">VRoid Studio</a></h3>
<h3 dir="auto"><a id="user-content-vtuber_unity" class="anchor" aria-hidden="true" href="#vtuber_unity"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><a href="https://github.com/kwea123/VTuber_Unity">VTuber_Unity</a></h3>
<p align="center" dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/kwea123/VTuber_Unity/blob/master/images/debug_gpu.gif?raw=true"><img src="https://github.com/kwea123/VTuber_Unity/raw/master/images/debug_gpu.gif?raw=true" data-animated-image="" style="max-width: 100%;"></a></p>
<h3 dir="auto"><a id="user-content-openvtuber" class="anchor" aria-hidden="true" href="#openvtuber"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><a href="https://github.com/1996scarlet/OpenVtuber">OpenVtuber</a></h3>
<p align="center" dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/83ad3e28fa8a9b51d5e30cdf745324b09ac97650aea38742c8e4806f9526bc91/68747470733a2f2f73332e617831782e636f6d2f323032302f31322f31322f72564f33464f2e676966"><img src="https://camo.githubusercontent.com/83ad3e28fa8a9b51d5e30cdf745324b09ac97650aea38742c8e4806f9526bc91/68747470733a2f2f73332e617831782e636f6d2f323032302f31322f31322f72564f33464f2e676966" style="max-width: 100%;"></a></p>
<hr>
<h2 dir="auto"><a id="user-content-hand-pose" class="anchor" aria-hidden="true" href="#hand-pose"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Hand Pose</h2>
<p dir="auto"><a href="https://codechina.csdn.net/mirrors/xinghaochen/awesome-hand-pose-estimation" rel="nofollow">Hand Pose Estimation papers</a></p>
<h3 dir="auto"><a id="user-content-hand3d" class="anchor" aria-hidden="true" href="#hand3d"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Hand3D</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/1705.01389" rel="nofollow">arxiv.org/abs/1705.01389</a><br>
<strong>Code:</strong> <a href="https://github.com/lmb-freiburg/hand3d">lmb-freiburg/hand3d</a><br>
<a target="_blank" rel="noopener noreferrer" href="https://github.com/lmb-freiburg/hand3d/blob/master/teaser.png?raw=true"><img src="https://github.com/lmb-freiburg/hand3d/raw/master/teaser.png?raw=true" alt="" style="max-width: 100%;"></a></p>
<h3 dir="auto"><a id="user-content-deehps" class="anchor" aria-hidden="true" href="#deehps"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>DeeHPS</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/1808.09208" rel="nofollow">arxiv.org/abs/1808.09208</a><br></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/81a5d5d7cb96a6e30732fdb9c05c8f753ce26aa1eeba8c6be736cf451edbac84/68747470733a2f2f7777772e7265736561726368676174652e6e65742f70726f66696c652f416c657869732d48656c6f69722f7075626c69636174696f6e2f3332383331303138392f6669677572652f666967312f41533a36393239303334313232343033383740313534323231323435353437352f612d416e2d6f766572766965772d6f662d6f75722d6d6574686f642d666f722d73696d756c74616e656f75732d33442d68616e642d706f73652d616e642d737572666163652d657374696d6174696f6e2d412e70706d"><img src="https://camo.githubusercontent.com/81a5d5d7cb96a6e30732fdb9c05c8f753ce26aa1eeba8c6be736cf451edbac84/68747470733a2f2f7777772e7265736561726368676174652e6e65742f70726f66696c652f416c657869732d48656c6f69722f7075626c69636174696f6e2f3332383331303138392f6669677572652f666967312f41533a36393239303334313232343033383740313534323231323435353437352f612d416e2d6f766572766965772d6f662d6f75722d6d6574686f642d666f722d73696d756c74616e656f75732d33442d68616e642d706f73652d616e642d737572666163652d657374696d6174696f6e2d412e70706d" alt="" data-canonical-src="https://www.researchgate.net/profile/Alexis-Heloir/publication/328310189/figure/fig1/AS:692903412240387@1542212455475/a-An-overview-of-our-method-for-simultaneous-3D-hand-pose-and-surface-estimation-A.ppm" style="max-width: 100%;"></a></p>
<h3 dir="auto"><a id="user-content-graphposegan" class="anchor" aria-hidden="true" href="#graphposegan"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>GraphPoseGAN</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/1912.01875" rel="nofollow">arxiv.org/abs/1912.01875</a><br></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/004cc5f0fbb3ad194f537e1b9dc9f1ce840ab13f12c37bd9c6dd529006692dc0/68747470733a2f2f6169322d73322d7075626c69632e73332e616d617a6f6e6177732e636f6d2f666967757265732f323031372d30382d30382f393437396132373866336336336235376232366562333165343437343461323338623131666565652f312d466967757265312d312e706e67"><img src="https://camo.githubusercontent.com/004cc5f0fbb3ad194f537e1b9dc9f1ce840ab13f12c37bd9c6dd529006692dc0/68747470733a2f2f6169322d73322d7075626c69632e73332e616d617a6f6e6177732e636f6d2f666967757265732f323031372d30382d30382f393437396132373866336336336235376232366562333165343437343461323338623131666565652f312d466967757265312d312e706e67" alt="" data-canonical-src="https://ai2-s2-public.s3.amazonaws.com/figures/2017-08-08/9479a278f3c63b57b26eb31e44744a238b11feee/1-Figure1-1.png" style="max-width: 100%;"></a></p>
<h3 dir="auto"><a id="user-content-3d-hand-shape" class="anchor" aria-hidden="true" href="#3d-hand-shape"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>3D Hand Shape</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/1903.00812" rel="nofollow">arxiv.org/abs/1903.00812</a><br>
<strong>Code:</strong> <a href="https://github.com/3d-hand-shape/hand-graph-cnn">https://github.com/3d-hand-shape/hand-graph-cnn</a><br></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/3d-hand-shape/hand-graph-cnn/blob/master/teaser.png?raw=true"><img src="https://github.com/3d-hand-shape/hand-graph-cnn/raw/master/teaser.png?raw=true" alt="" style="max-width: 100%;"></a></p>
<hr>
<h3 dir="auto"><a id="user-content-facebook-interhand26m" class="anchor" aria-hidden="true" href="#facebook-interhand26m"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>FaceBook InterHand2.6M</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/2008.09309" rel="nofollow">InterHand2.6M: A Dataset and Baseline for 3D Interacting Hand Pose Estimation from a Single RGB Image
</a><br>
<strong>Code:</strong> <a href="https://github.com/facebookresearch/InterHand2.6M">facebookresearch/InterHand2.6M</a><br></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/facebookresearch/InterHand2.6M/blob/main/assets/teaser.gif?raw=true"><img src="https://github.com/facebookresearch/InterHand2.6M/raw/main/assets/teaser.gif?raw=true" alt="" data-animated-image="" style="max-width: 100%;"></a></p>
<hr>
<h3 dir="auto"><a id="user-content-frankmocap-fast-monocular-3d-hand-and-body-motion-capture-by-regression-and-integration" class="anchor" aria-hidden="true" href="#frankmocap-fast-monocular-3d-hand-and-body-motion-capture-by-regression-and-integration"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>FrankMocap: Fast Monocular 3D Hand and Body Motion Capture by Regression and Integration</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/2008.08324" rel="nofollow">arxiv.org/abs/2008.08324</a><br>
<strong>Code:</strong> <a href="https://github.com/facebookresearch/frankmocap">facebookresearch/frankmocap</a><br></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/681ceb7f7a779fbf3d427ec094c189eb7f2add28af3da6881ced1ddc6f356eda/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f313336362f312a53495351687066387070686e6f6233546a542d6857512e706e67"><img src="https://camo.githubusercontent.com/681ceb7f7a779fbf3d427ec094c189eb7f2add28af3da6881ced1ddc6f356eda/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f313336362f312a53495351687066387070686e6f6233546a542d6857512e706e67" alt="" data-canonical-src="https://miro.medium.com/max/1366/1*SISQhpf8pphnob3TjT-hWQ.png" style="max-width: 100%;"></a>
<a target="_blank" rel="noopener noreferrer" href="https://github.com/jhugestar/jhugestar.github.io/blob/master/img/frankmocap_wholebody.gif?raw=true"><img src="https://github.com/jhugestar/jhugestar.github.io/raw/master/img/frankmocap_wholebody.gif?raw=true" alt="" data-animated-image="" style="max-width: 100%;"></a></p>
<hr>
<h3 dir="auto"><a id="user-content-a-skeleton-driven-neural-occupancy-representation-for-articulated-hands" class="anchor" aria-hidden="true" href="#a-skeleton-driven-neural-occupancy-representation-for-articulated-hands"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>A Skeleton-Driven Neural Occupancy Representation for Articulated Hands</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/2109.11399" rel="nofollow">arxiv.org/abs/2109.11399</a><br></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/c4024cd9a3ff7723fb51ce0c25877fb553d7b235e1ce07db1d8a82e38664ff8d/68747470733a2f2f64336937317861627572686434322e636c6f756466726f6e742e6e65742f663662626262396135303762303062626230303365353564383838363033636364663437613736322f372d466967757265352d312e706e67"><img src="https://camo.githubusercontent.com/c4024cd9a3ff7723fb51ce0c25877fb553d7b235e1ce07db1d8a82e38664ff8d/68747470733a2f2f64336937317861627572686434322e636c6f756466726f6e742e6e65742f663662626262396135303762303062626230303365353564383838363033636364663437613736322f372d466967757265352d312e706e67" alt="" data-canonical-src="https://d3i71xaburhd42.cloudfront.net/f6bbbb9a507b00bbb003e55d888603ccdf47a762/7-Figure5-1.png" style="max-width: 100%;"></a></p>
<h3 dir="auto"><a id="user-content-towards-unconstrained-joint-hand-object-reconstruction-from-rgb-videos" class="anchor" aria-hidden="true" href="#towards-unconstrained-joint-hand-object-reconstruction-from-rgb-videos"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Towards unconstrained joint hand-object reconstruction from RGB videos</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/2108.07044" rel="nofollow">arxiv.org/abs/2108.07044</a><br>
<strong>Code:</strong> <a href="https://github.com/hassony2/homan">hassony2/homan</a><br></p>
<table>
  <tbody><tr>
  <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/hassony2/homan/raw/master/5900_in.gif?raw=True"><img src="https://github.com/hassony2/homan/raw/master/5900_in.gif?raw=True" data-animated-image="" style="max-width: 100%;"></a></td>
  <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/hassony2/homan/raw/master/5900_cam.gif?raw=True"><img src="https://github.com/hassony2/homan/raw/master/5900_cam.gif?raw=True" data-animated-image="" style="max-width: 100%;"></a></td>
  <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/hassony2/homan/raw/master/0011.gif?raw=True"><img src="https://github.com/hassony2/homan/raw/master/0011.gif?raw=True" data-animated-image="" style="max-width: 100%;"></a></td>
  </tr>
</tbody></table>
<h3 dir="auto"><a id="user-content-fast-monocular-hand-pose-estimation-on-embedded-systems" class="anchor" aria-hidden="true" href="#fast-monocular-hand-pose-estimation-on-embedded-systems"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Fast Monocular Hand Pose Estimation on Embedded Systems</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/2102.07067" rel="nofollow">arxiv.org/abs/2102.07067</a><br></p>
<h3 dir="auto"><a id="user-content-recent-advances-in-3d-object-and-hand-pose-estimation" class="anchor" aria-hidden="true" href="#recent-advances-in-3d-object-and-hand-pose-estimation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Recent Advances in 3D Object and Hand Pose Estimation</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/2006.05927" rel="nofollow">arxiv.org/abs/2006.05927</a><br></p>
<hr>
<h2 dir="auto"><a id="user-content-object-pose" class="anchor" aria-hidden="true" href="#object-pose"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Object Pose</h2>
<h3 dir="auto"><a id="user-content-benchmark-for-6d-object-pose-" class="anchor" aria-hidden="true" href="#benchmark-for-6d-object-pose-"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><a href="https://bop.felk.cvut.cz/challenges/bop-challenge-2019/" rel="nofollow">Benchmark for 6D Object Pose </a></h3>
<p dir="auto"><strong>Core datasets:</strong><br></p>
<table>
  <tbody><tr>
  <td><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/ae25310ab0ab583bf44c2bc768854f6bb7ac4a3ae4dda3029fb09a91032c046e/68747470733a2f2f626f702e66656c6b2e637675742e637a2f6d656469612f6c6d6f5f7468756d625f67745f745a38727033642e6a7067"><img width="160" height="120" src="https://camo.githubusercontent.com/ae25310ab0ab583bf44c2bc768854f6bb7ac4a3ae4dda3029fb09a91032c046e/68747470733a2f2f626f702e66656c6b2e637675742e637a2f6d656469612f6c6d6f5f7468756d625f67745f745a38727033642e6a7067" data-canonical-src="https://bop.felk.cvut.cz/media/lmo_thumb_gt_tZ8rp3d.jpg" style="max-width: 100%;"></a></td>
  <td><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/95a931e42c0d8c53d7beba3ee0306f5e844bd907393cb7d9339bf69b924fad53/68747470733a2f2f626f702e66656c6b2e637675742e637a2f6d656469612f746c6573735f6c6d5f7468756d625f67745f637976414f68522e6a7067"><img width="160" height="120" src="https://camo.githubusercontent.com/95a931e42c0d8c53d7beba3ee0306f5e844bd907393cb7d9339bf69b924fad53/68747470733a2f2f626f702e66656c6b2e637675742e637a2f6d656469612f746c6573735f6c6d5f7468756d625f67745f637976414f68522e6a7067" data-canonical-src="https://bop.felk.cvut.cz/media/tless_lm_thumb_gt_cyvAOhR.jpg" style="max-width: 100%;"></a></td>
  <td><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/4cc1adc69ddf71ac5126373706135ff490b76c31e6d35f33b30e22de746de410/68747470733a2f2f626f702e66656c6b2e637675742e637a2f6d656469612f7475646c5f7468756d625f67745f746a45797857382e6a7067"><img width="160" height="120" src="https://camo.githubusercontent.com/4cc1adc69ddf71ac5126373706135ff490b76c31e6d35f33b30e22de746de410/68747470733a2f2f626f702e66656c6b2e637675742e637a2f6d656469612f7475646c5f7468756d625f67745f746a45797857382e6a7067" data-canonical-src="https://bop.felk.cvut.cz/media/tudl_thumb_gt_tjEyxW8.jpg" style="max-width: 100%;"></a></td>
  <td><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/10a497162e4e2ed4facf796933c8263f021e4e6677bb01c610ea845c83632b38/68747470733a2f2f626f702e66656c6b2e637675742e637a2f6d656469612f696362696e5f7468756d625f67742e6a7067"><img width="160" height="120" src="https://camo.githubusercontent.com/10a497162e4e2ed4facf796933c8263f021e4e6677bb01c610ea845c83632b38/68747470733a2f2f626f702e66656c6b2e637675742e637a2f6d656469612f696362696e5f7468756d625f67742e6a7067" data-canonical-src="https://bop.felk.cvut.cz/media/icbin_thumb_gt.jpg" style="max-width: 100%;"></a></td>
  <td><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/4495ac438c459dd3e264bc68be8c4f9b707027ae124c5be2f0ec39a824bb304a/68747470733a2f2f626f702e66656c6b2e637675742e637a2f6d656469612f69746f64645f7468756d625f6774332e6a7067"><img width="160" height="120" src="https://camo.githubusercontent.com/4495ac438c459dd3e264bc68be8c4f9b707027ae124c5be2f0ec39a824bb304a/68747470733a2f2f626f702e66656c6b2e637675742e637a2f6d656469612f69746f64645f7468756d625f6774332e6a7067" data-canonical-src="https://bop.felk.cvut.cz/media/itodd_thumb_gt3.jpg" style="max-width: 100%;"></a></td>
  <td><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/4582663c975b1801d6cb4a75dd2fbe72762c0e391b7e993cd72f5ae52da2f377/68747470733a2f2f626f702e66656c6b2e637675742e637a2f6d656469612f68625f7468756d625f67742e6a7067"><img width="160" height="120" src="https://camo.githubusercontent.com/4582663c975b1801d6cb4a75dd2fbe72762c0e391b7e993cd72f5ae52da2f377/68747470733a2f2f626f702e66656c6b2e637675742e637a2f6d656469612f68625f7468756d625f67742e6a7067" data-canonical-src="https://bop.felk.cvut.cz/media/hb_thumb_gt.jpg" style="max-width: 100%;"></a></td>
  <td><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/989b41972469190ecf1f1e797905d39c6e64acbd22c125e00e536de5ec36e5d8/68747470733a2f2f626f702e66656c6b2e637675742e637a2f6d656469612f796362765f7468756d625f6774322e6a7067"><img width="160" height="120" src="https://camo.githubusercontent.com/989b41972469190ecf1f1e797905d39c6e64acbd22c125e00e536de5ec36e5d8/68747470733a2f2f626f702e66656c6b2e637675742e637a2f6d656469612f796362765f7468756d625f6774322e6a7067" data-canonical-src="https://bop.felk.cvut.cz/media/ycbv_thumb_gt2.jpg" style="max-width: 100%;"></a></td>
  </tr>
  <tr>
  <td align="center"><a href="https://bop.felk.cvut.cz/datasets/#LM-O" rel="nofollow">LM-O</a></td>
  <td align="center"><a href="https://bop.felk.cvut.cz/datasets/#T-LESS" rel="nofollow">T-LESS</a></td>
  <td align="center"><a href="https://bop.felk.cvut.cz/datasets/#TUD-L" rel="nofollow">TUD-L</a></td>
  <td align="center"><a href="https://bop.felk.cvut.cz/datasets/#IC-BIN" rel="nofollow">IC-BIN</a></td>
  <td align="center"><a href="https://bop.felk.cvut.cz/datasets/#ITODD" rel="nofollow">ITODD</a></td>
  <td align="center"><a href="https://bop.felk.cvut.cz/datasets/#HB" rel="nofollow">HB</a></td>
  <td align="center"><a href="https://bop.felk.cvut.cz/datasets/#YCB-V" rel="nofollow">YCB-V</a></td>
  </tr>
</tbody></table>
**Other datasets:** 
<a href="https://bop.felk.cvut.cz/datasets/#LM" rel="nofollow">LM</a>, 
<a href="https://bop.felk.cvut.cz/datasets/#RU-APC" rel="nofollow">RU-APC</a>,
<a href="https://bop.felk.cvut.cz/datasets/#IC-MI" rel="nofollow">IC-MI</a>,
<a href="https://bop.felk.cvut.cz/datasets/#TYO-L" rel="nofollow">TYO-L</a>.
<hr>
<h3 dir="auto"><a id="user-content-real-time-seamless-single-shot-6d-object-pose-prediction-yolo-6d" class="anchor" aria-hidden="true" href="#real-time-seamless-single-shot-6d-object-pose-prediction-yolo-6d"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Real-Time Seamless Single Shot 6D Object Pose Prediction (YOLO-6D)</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/1711.08848" rel="nofollow">arxiv.org/abs/1711.08848</a><br>
<strong>Code:</strong> <a href="https://github.com/microsoft/singleshotpose">microsoft/singleshotpose</a><br></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/803dd24670ed987bc9477d7bf7b63dd54509da2fe945de35e123a82c90006d6a/68747470733a2f2f6274656b696e2e6769746875622e696f2f73696e676c655f73686f745f706f73652e706e67"><img src="https://camo.githubusercontent.com/803dd24670ed987bc9477d7bf7b63dd54509da2fe945de35e123a82c90006d6a/68747470733a2f2f6274656b696e2e6769746875622e696f2f73696e676c655f73686f745f706f73652e706e67" alt="" style="max-width: 100%;"></a></p>
<hr>
<h3 dir="auto"><a id="user-content-posecnn" class="anchor" aria-hidden="true" href="#posecnn"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>PoseCNN</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/1711.00199" rel="nofollow">arxiv.org/abs/1711.00199</a><br>
<strong>Code:</strong> <a href="https://github.com/yuxng/PoseCNN">yuxng/PoseCNN</a><br></p>
<p dir="auto"><a href="https://youtu.be/ih0cCTxO96Y" rel="nofollow"><img src="https://camo.githubusercontent.com/f332b3b33da74f38cce06e4cf835b6fd35b84d150b16f0a3c48ef0d0113448c9/687474703a2f2f7975786e672e6769746875622e696f2f506f7365434e4e2e706e67" alt="PoseCNN" data-canonical-src="http://yuxng.github.io/PoseCNN.png" style="max-width: 100%;"></a></p>
<hr>
<h3 dir="auto"><a id="user-content-deepim" class="anchor" aria-hidden="true" href="#deepim"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>DeepIM</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/1804.00175" rel="nofollow">arxiv.org/abs/1804.00175</a><br>
<strong>Code:</strong> <a href="https://github.com/liyi14/mx-DeepIM">liyi14/mx-DeepIM</a><br></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/liyi14/mx-DeepIM/blob/master/assets/net_structure.png?raw=tru"><img src="https://github.com/liyi14/mx-DeepIM/raw/master/assets/net_structure.png?raw=tru" alt="" style="max-width: 100%;"></a></p>
<hr>
<h3 dir="auto"><a id="user-content-segmentation-driven-pose" class="anchor" aria-hidden="true" href="#segmentation-driven-pose"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Segmentation-driven Pose</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/1812.02541" rel="nofollow">arxiv.org/abs/1812.02541</a><br>
<strong>Code:</strong> <a href="https://github.com/cvlab-epfl/segmentation-driven-pose">cvlab-epfl/segmentation-driven-pose</a><br></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/cvlab-epfl/segmentation-driven-pose/blob/master/images/fig1.jpg?raw=true"><img src="https://github.com/cvlab-epfl/segmentation-driven-pose/raw/master/images/fig1.jpg?raw=true" alt="" style="max-width: 100%;"></a></p>
<hr>
<h3 dir="auto"><a id="user-content-dpod" class="anchor" aria-hidden="true" href="#dpod"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>DPOD</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/1902.11020" rel="nofollow">arxiv.org/abs/1902.11020</a><br>
<strong>Code:</strong> <a href="https://github.com/yashs97/DPOD">yashs97/DPOD</a><br></p>
<table>
  <tbody><tr>
  <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/yashs97/DPOD/blob/master/demo_results/demo1.png?raw=true"><img src="https://github.com/yashs97/DPOD/raw/master/demo_results/demo1.png?raw=true" style="max-width: 100%;"></a></td>
  <td><a target="_blank" rel="noopener noreferrer" href="https://github.com/yashs97/DPOD/blob/master/demo_results/demo2.png?raw=true"><img src="https://github.com/yashs97/DPOD/raw/master/demo_results/demo2.png?raw=true" style="max-width: 100%;"></a></td>
  </tr>
</tbody></table>
![](<a href="https://d3i71xaburhd42.cloudfront.net/efae64551ff0b38fb6ac938727a001a9892be67f/4-Figure2-1.png" rel="nofollow">https://d3i71xaburhd42.cloudfront.net/efae64551ff0b38fb6ac938727a001a9892be67f/4-Figure2-1.png</a>)
<hr>
<h3 dir="auto"><a id="user-content-ho-3d_v3-dataset" class="anchor" aria-hidden="true" href="#ho-3d_v3-dataset"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>HO-3D_v3 Dataset</h3>
<p dir="auto"><strong>Paper:</strong> <a href="https://arxiv.org/abs/2107.00887" rel="nofollow">arxiv.org/abs/2107.00887</a><br>
<strong>Github:</strong> <a href="https://github.com/shreyashampali/ho3d">shreyashampali/ho3d</a><br>
HO-3D is a dataset with 3D pose annotations for hand and object under severe occlusions from each other.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/shreyashampali/ho3d/blob/master/teaser.png?raw=true"><img src="https://github.com/shreyashampali/ho3d/raw/master/teaser.png?raw=true" alt="" style="max-width: 100%;"></a></p>
<hr>
<h2 dir="auto"><a id="user-content-exercises-of-pose-estimation" class="anchor" aria-hidden="true" href="#exercises-of-pose-estimation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Exercises of Pose Estimation</h2>
<h3 dir="auto"><a id="user-content-bodypix" class="anchor" aria-hidden="true" href="#bodypix"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>BodyPix</h3>
<p dir="auto"><strong>Kaggle:</strong> <a href="https://kaggle.com/rkuo2000/BodyPix" rel="nofollow">rkuo2000/BodyPix</a><br>
<a target="_blank" rel="noopener noreferrer" href="https://github.com/rkuo2000/AI-course/blob/gh-pages/images/BodyPix_results.png?raw=true"><img src="https://github.com/rkuo2000/AI-course/raw/gh-pages/images/BodyPix_results.png?raw=true" alt="" style="max-width: 100%;"></a></p>
<hr>
<h3 dir="auto"><a id="user-content-posenet-1" class="anchor" aria-hidden="true" href="#posenet-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>PoseNet</h3>
<p dir="auto"><strong>Kaggle:</strong> <a href="https://www.kaggle.com/rkuo2000/posenet-pytorch" rel="nofollow">rkuo2000/posenet-pytorch</a><br>
<a target="_blank" rel="noopener noreferrer" href="https://github.com/rkuo2000/AI-course/blob/gh-pages/images/PoseNet_keypoints.png?raw=true"><img src="https://github.com/rkuo2000/AI-course/raw/gh-pages/images/PoseNet_keypoints.png?raw=true" alt="" style="max-width: 100%;"></a>
<strong>Kaggle:</strong> <a href="https://www.kaggle.com/rkuo2000/posenet-human-pose" rel="nofollow">rkuo2000/posenet-human-pose</a><br>
<a target="_blank" rel="noopener noreferrer" href="https://github.com/rkuo2000/AI-course/blob/gh-pages/images/PoseNet_bodylines.png?raw=true"><img src="https://github.com/rkuo2000/AI-course/raw/gh-pages/images/PoseNet_bodylines.png?raw=true" alt="" style="max-width: 100%;"></a></p>
<hr>
<h3 dir="auto"><a id="user-content-mmpose-1" class="anchor" aria-hidden="true" href="#mmpose-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>MMPose</h3>
<p dir="auto"><strong>Kaggle:</strong><a href="https://www.kaggle.com/rkuo2000/mmpose" rel="nofollow">rkuo2000/MMPose</a> <br></p>
<h4 dir="auto"><a id="user-content-2d-human-pose" class="anchor" aria-hidden="true" href="#2d-human-pose"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>2D Human Pose</h4>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/open-mmlab/mmpose/blob/master/demo/resources/demo_coco.gif?raw=true"><img src="https://github.com/open-mmlab/mmpose/raw/master/demo/resources/demo_coco.gif?raw=true" alt="" data-animated-image="" style="max-width: 100%;"></a></p>
<h4 dir="auto"><a id="user-content-2d-human-whole-body" class="anchor" aria-hidden="true" href="#2d-human-whole-body"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>2D Human Whole-Body</h4>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://user-images.githubusercontent.com/9464825/95552839-00a61080-0a40-11eb-818c-b8dad7307217.gif"><img src="https://user-images.githubusercontent.com/9464825/95552839-00a61080-0a40-11eb-818c-b8dad7307217.gif" alt="" data-animated-image="" style="max-width: 100%;"></a></p>
<h4 dir="auto"><a id="user-content-2d-hand-pose" class="anchor" aria-hidden="true" href="#2d-hand-pose"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>2D Hand Pose</h4>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://user-images.githubusercontent.com/11788150/109098558-8c54db00-775c-11eb-8966-85df96b23dc5.gif"><img src="https://user-images.githubusercontent.com/11788150/109098558-8c54db00-775c-11eb-8966-85df96b23dc5.gif" alt="" data-animated-image="" style="max-width: 100%;"></a></p>
<h4 dir="auto"><a id="user-content-2d-face-keypoints" class="anchor" aria-hidden="true" href="#2d-face-keypoints"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>2D Face Keypoints</h4>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://user-images.githubusercontent.com/11788150/109144943-ccd44900-779c-11eb-9e9d-8682e7629654.gif"><img src="https://user-images.githubusercontent.com/11788150/109144943-ccd44900-779c-11eb-9e9d-8682e7629654.gif" alt="" data-animated-image="" style="max-width: 100%;"></a></p>
<h4 dir="auto"><a id="user-content-3d-human-pose" class="anchor" aria-hidden="true" href="#3d-human-pose"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>3D Human Pose</h4>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://user-images.githubusercontent.com/15977946/118820606-02df2000-b8e9-11eb-9984-b9228101e780.gif"><img src="https://user-images.githubusercontent.com/15977946/118820606-02df2000-b8e9-11eb-9984-b9228101e780.gif" alt="" data-animated-image="" style="max-width: 100%;"></a></p>
<h4 dir="auto"><a id="user-content-2d-pose-tracking" class="anchor" aria-hidden="true" href="#2d-pose-tracking"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>2D Pose Tracking</h4>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://user-images.githubusercontent.com/11788150/109099201-a93dde00-775d-11eb-9624-f9676fc0e478.gif"><img src="https://user-images.githubusercontent.com/11788150/109099201-a93dde00-775d-11eb-9624-f9676fc0e478.gif" alt="" data-animated-image="" style="max-width: 100%;"></a></p>
<h4 dir="auto"><a id="user-content-2d-animal-pose" class="anchor" aria-hidden="true" href="#2d-animal-pose"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>2D Animal Pose</h4>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://user-images.githubusercontent.com/11788150/114201893-4446ec00-9989-11eb-808b-5718c47c7b23.gif"><img src="https://user-images.githubusercontent.com/11788150/114201893-4446ec00-9989-11eb-808b-5718c47c7b23.gif" alt="" data-animated-image="" style="max-width: 100%;"></a></p>
<h4 dir="auto"><a id="user-content-3d-hand-pose" class="anchor" aria-hidden="true" href="#3d-hand-pose"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>3D Hand Pose</h4>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://user-images.githubusercontent.com/28900607/121288285-b8fcbf00-c915-11eb-98e4-ba846de12987.gif"><img src="https://user-images.githubusercontent.com/28900607/121288285-b8fcbf00-c915-11eb-98e4-ba846de12987.gif" alt="" data-animated-image="" style="max-width: 100%;"></a></p>
<h4 dir="auto"><a id="user-content-webcam-effect" class="anchor" aria-hidden="true" href="#webcam-effect"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>WebCam Effect</h4>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://user-images.githubusercontent.com/15977946/124059525-ce20c580-da5d-11eb-8e4a-2d96cd31fe9f.gif"><img src="https://user-images.githubusercontent.com/15977946/124059525-ce20c580-da5d-11eb-8e4a-2d96cd31fe9f.gif" alt="" data-animated-image="" style="max-width: 100%;"></a></p>
<hr>
<h3 dir="auto"><a id="user-content-openpose-1" class="anchor" aria-hidden="true" href="#openpose-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>OpenPose</h3>
<p dir="auto"><strong>Kaggle:</strong> <a href="https://github.com/rkuo2000/openpose-pytorch">rkuo2000/openpose-pytorch</a><br>
<a target="_blank" rel="noopener noreferrer" href="https://github.com/rkuo2000/AI-course/blob/gh-pages/images/OpenPose_pytorch_racers.png?raw=true"><img src="https://github.com/rkuo2000/AI-course/raw/gh-pages/images/OpenPose_pytorch_racers.png?raw=true" alt="" style="max-width: 100%;"></a>
<a target="_blank" rel="noopener noreferrer" href="https://github.com/rkuo2000/AI-course/blob/gh-pages/images/OpenPose_pytorch_fall1.png?raw=true"><img src="https://github.com/rkuo2000/AI-course/raw/gh-pages/images/OpenPose_pytorch_fall1.png?raw=true" alt="" style="max-width: 100%;"></a></p>
<hr>
<h3 dir="auto"><a id="user-content-pose-recognition-姿態辨識" class="anchor" aria-hidden="true" href="#pose-recognition-姿態辨識"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Pose Recognition (姿態辨識)</h3>
<p dir="auto"><strong>專題實作步驟:</strong></p>
<ol dir="auto">
<li>建立身體動作之姿態照片資料集 (例如：5 poses , take 20 pictures of each pose)<br></li>
<li>始用<strong>MMPose</strong> 辨識出照片中的各姿勢之身體關鍵點 (use MMPose convert 16 keypoints (x,y) of each pose)<br></li>
<li>產生姿態關鍵點資料集 x_train.append(pose_keypoints) ( x_train.shape = (20x5, 16, 2), y_train.shape= (20x5, 1) )<br></li>
<li>建立DNN模型並訓練模型, 然後下載模型檔<code>pose_dnn.h5</code>至PC <br></li>
<li>於PC建立帶camera輸入之服務器程式, 載入模型<code>pose_dnn.h5</code>進行姿態動作辨識 <br></li>
</ol>
<p dir="auto"><strong>模型建構與訓練之程式樣本</strong> (PC or Kaggle)<br></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="input_shape=(16,2)
num_classes=5

inputs = layers.Input(shape=input_shape)
x = layers.Dense(128)(inputs)
outputs = layers.Dense(num_classes, activation=&quot;softmax&quot;)(x)
model = models.Model(inputs=inputs, outputs=outputs)

models.compile(loss = 'categorical_crossentropy', optimizer = 'adam' , metrics = ['accuracy'])

history = model.fit(x_train, y_train, batch_size=1, epochs=20, validation_data=(x_test, y_test))
models.save_model(model, 'pose_dnn.h5')"><pre class="notranslate"><code>input_shape=(16,2)
num_classes=5

inputs = layers.Input(shape=input_shape)
x = layers.Dense(128)(inputs)
outputs = layers.Dense(num_classes, activation="softmax")(x)
model = models.Model(inputs=inputs, outputs=outputs)

models.compile(loss = 'categorical_crossentropy', optimizer = 'adam' , metrics = ['accuracy'])

history = model.fit(x_train, y_train, batch_size=1, epochs=20, validation_data=(x_test, y_test))
models.save_model(model, 'pose_dnn.h5')
</code></pre></div>
<p dir="auto"><strong>姿態辨識服務器之程式樣本</strong> (PC with Camera)<br></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="model = models.load_model('models/pose_dnn.h5')
labels = ['stand', 'raise-right-arm', 'raise-left-arm', 'cross arms','both-arms-left']

cap = cv2.VideoCapture(0)

while(cap.isOpened()):
    ret, frame = cap.read()
    image = cv2.cvtColor(frame,cv2.COLOR_BGR2RGB)
    
    mmdet_results = inference_detector(det_model, image) # 人物偵測產生BBox
    person_results = process_mmdet_results(mmdet_results, args.det_cat_id) # 記住人物之BBox  
    pose_results, returned_outputs = inference_top_down_pose_model(...) # 感測姿態產生pose keypoints
    
    x_test = np.array(preson_results).reshape(1,16,2) # 將Keypoints List 轉成 numpy Array
    preds = model.fit(x_test) # 辨識姿態動作
    maxindex = int(np.argmax(preds))
    txt = labels[maxindex]
    print(txt)"><pre class="notranslate"><code>model = models.load_model('models/pose_dnn.h5')
labels = ['stand', 'raise-right-arm', 'raise-left-arm', 'cross arms','both-arms-left']

cap = cv2.VideoCapture(0)

while(cap.isOpened()):
    ret, frame = cap.read()
    image = cv2.cvtColor(frame,cv2.COLOR_BGR2RGB)
    
    mmdet_results = inference_detector(det_model, image) # 人物偵測產生BBox
    person_results = process_mmdet_results(mmdet_results, args.det_cat_id) # 記住人物之BBox  
    pose_results, returned_outputs = inference_top_down_pose_model(...) # 感測姿態產生pose keypoints
    
    x_test = np.array(preson_results).reshape(1,16,2) # 將Keypoints List 轉成 numpy Array
    preds = model.fit(x_test) # 辨識姿態動作
    maxindex = int(np.argmax(preds))
    txt = labels[maxindex]
    print(txt)
</code></pre></div>
<hr>
<h3 dir="auto"><a id="user-content-head-pose-estimation-1" class="anchor" aria-hidden="true" href="#head-pose-estimation-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Head Pose Estimation</h3>
<p dir="auto"><strong>Kaggle:</strong> <a href="https://kaggle.com/rkuo2000/head-pose-estimation" rel="nofollow">rkuo2000/head-pose-estimation</a><br></p>
&lt;iframe width="652" height="489" src="<a href="https://www.youtube.com/embed/BHwHmCUHRyQ" rel="nofollow">https://www.youtube.com/embed/BHwHmCUHRyQ</a>" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen&gt;&lt;/iframe&gt;
<hr>
<h3 dir="auto"><a id="user-content-vtuber-unity" class="anchor" aria-hidden="true" href="#vtuber-unity"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>VTuber-Unity</h3>
<p dir="auto"><strong>Head-Pose-Estimation + Face-Alignment + GazeTracking</strong><br></p>
<p dir="auto">Build-up Steps:</p>
<ol dir="auto">
<li>Create a character: <strong><a href="https://vroid.com/studio" rel="nofollow">VRoid Studio</a></strong></li>
<li>Synchronize the face: <strong><a href="https://github.com/kwea123/VTuber_Unity">VTuber_Unity</a></strong></li>
<li>Take video: <strong><a href="https://obsproject.com/download" rel="nofollow">OBS Studio</a></strong></li>
<li>Post-processing:</li>
</ol>
<ul dir="auto">
<li>Auto-subtitle: <strong><a href="https://github.com/kwea123/autosub">Autosub</a></strong></li>
<li>Auto-subtitle in live stream: <strong><a href="https://github.com/kwea123/Unity_live_caption">Unity_live_caption</a></strong></li>
<li>Encode the subtitle into video: <strong><a href="https://maruko.appinn.me/" rel="nofollow">小丸工具箱</a></strong></li>
</ul>
<ol start="5" dir="auto">
<li>Upload: YouTube</li>
<li>[Optional] Install CUDA &amp; CuDNN to enable GPU acceleration</li>
<li>To Run <br>
<code>$git clone https://github.com/kwea123/VTuber_Unity</code> <br>
<code>$python demo.py --debug --cpu</code> <br></li>
</ol>
<p align="center" dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/kwea123/VTuber_Unity/blob/master/images/debug_gpu.gif?raw=true"><img src="https://github.com/kwea123/VTuber_Unity/raw/master/images/debug_gpu.gif?raw=true" data-animated-image="" style="max-width: 100%;"></a></p>
<hr>
<h3 dir="auto"><a id="user-content-openvtuber-1" class="anchor" aria-hidden="true" href="#openvtuber-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>OpenVtuber</h3>
<p dir="auto">Build-up Steps:</p>
<ul dir="auto">
<li>Repro <a href="https://github.com/1996scarlet/OpenVtuber">Github</a><br>
<code>$git clone https://github.com/1996scarlet/OpenVtuber</code><br>
<code>$cd OpenVtuber</code><br>
<code>$pip3 install –r requirements.txt</code><br></li>
<li>Install node.js for Windows <br></li>
<li>run Socket-IO Server <br>
<code>$cd NodeServer</code> <br>
<code>$npm install express socket.io</code> <br>
<code>$node. index.js</code> <br></li>
<li>Open a browser at  <a href="http://127.0.0.1:6789/kizuna" rel="nofollow">http://127.0.0.1:6789/kizuna</a> <br></li>
<li>PythonClient with Webcam <br>
<code>$cd ../PythonClient</code> <br>
<code>$python3 vtuber_link_start.py</code> <br></li>
</ul>
<p align="center" dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/83ad3e28fa8a9b51d5e30cdf745324b09ac97650aea38742c8e4806f9526bc91/68747470733a2f2f73332e617831782e636f6d2f323032302f31322f31322f72564f33464f2e676966"><img src="https://camo.githubusercontent.com/83ad3e28fa8a9b51d5e30cdf745324b09ac97650aea38742c8e4806f9526bc91/68747470733a2f2f73332e617831782e636f6d2f323032302f31322f31322f72564f33464f2e676966" style="max-width: 100%;"></a></p>
<hr>
<h3 dir="auto"><a id="user-content-hand-pose-1" class="anchor" aria-hidden="true" href="#hand-pose-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Hand Pose</h3>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/facebookresearch/InterHand2.6M/blob/main/assets/teaser.gif?raw=true"><img src="https://github.com/facebookresearch/InterHand2.6M/raw/main/assets/teaser.gif?raw=true" alt="" data-animated-image="" style="max-width: 100%;"></a>
<strong>Dataset:</strong> <a href="https://github.com/facebookresearch/InterHand2.6M">InterHand2.6M</a><br></p>
<ol dir="auto">
<li>Download pre-trained InterNet from <a href="https://drive.google.com/drive/folders/1BET1f5p2-1OBOz6aNLuPBAVs_9NLz5Jo?usp=sharing" rel="nofollow">here</a></li>
<li>Put the model at <code>demo</code> folder</li>
<li>Go to <code>demo</code> folder and edit <code>bbox</code> in <a href="https://github.com/facebookresearch/InterHand2.6M/blob/5de679e614151ccfd140f0f20cc08a5f94d4b147/demo/demo.py#L74">here</a></li>
<li>run <code>python demo.py --gpu 0 --test_epoch 20</code></li>
<li>You can see <code>result_2D.jpg</code> and 3D viewer.</li>
</ol>
<p dir="auto"><strong>Camera positios visualization demo</strong></p>
<ol dir="auto">
<li><code>cd tool/camera_visualize</code></li>
<li>Run <code>python camera_visualize.py</code></li>
</ol>
<br>
<br>
<p dir="auto"><em>This site was last updated {{ site.time | date: "%B %d, %Y" }}.</em></p>
</article>
  </div>

    </div>

  </readme-toc>

  

  <details class="details-reset details-overlay details-overlay-dark" id="jumpto-line-details-dialog">
    <summary data-hotkey="l" aria-label="Jump to line"></summary>
    <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast linejump" aria-label="Jump to line">
      <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="js-jump-to-line-form Box-body d-flex" data-turbo="false" action="" accept-charset="UTF-8" method="get">
        <input class="form-control flex-auto mr-3 linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
          <button data-close-dialog="" type="submit" data-view-component="true" class="btn">    Go
</button>
</form>    </details-dialog>
  </details>



    <div class="pt-3" >
      <details class="details-reset details-overlay details-overlay-dark " >
                <summary data-view-component="true" class="btn-link">    Give feedback
</summary>

  <details-dialog
    class="Box d-flex flex-column anim-fade-in fast Box--overlay overflow-visible"
      aria-label="Provide feedback"
      src="/sean207cc/AI-course/repos/code_nav_survey"
      
    >
    <div class="Box-header">
      <button class="Box-btn-octicon btn-octicon float-right" type="button" aria-label="Close dialog" data-close-dialog>
        <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path>
</svg>
      </button>
        <h1 class="Box-title" >Provide feedback</h1>
    </div>
      <div class="Box-body overflow-auto">
                  <include-fragment>
            <svg style="box-sizing: content-box; color: var(--color-icon-primary);" width="32" height="32" viewBox="0 0 16 16" fill="none" data-view-component="true" class="my-3 mx-auto d-block anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" />
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke" />
</svg>
          </include-fragment>

      </div>
  </details-dialog>
</details>
    </div>
</div>

  </div>


  </div>

  </turbo-frame>


    </main>
  </div>

  </div>

          <footer class="footer width-full container-xl p-responsive">
  <h2 class='sr-only'>Footer</h2>

  <div class="position-relative d-flex flex-items-center pb-2 f6 color-fg-muted border-top color-border-muted flex-column-reverse flex-lg-row flex-wrap flex-lg-nowrap mt-6 pt-6">
    <div class="list-style-none d-flex flex-wrap col-0 col-lg-2 flex-justify-start flex-lg-justify-between mb-2 mb-lg-0">
      <div class="mt-2 mt-lg-0 d-flex flex-items-center">
        <a aria-label="Homepage" title="GitHub" class="footer-octicon mr-2" href="https://github.com">
          <svg aria-hidden="true" height="24" viewBox="0 0 16 16" version="1.1" width="24" data-view-component="true" class="octicon octicon-mark-github">
    <path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path>
</svg>
</a>        <span>
        &copy; 2022 GitHub, Inc.
        </span>
      </div>
    </div>

    <nav aria-label='footer' class="col-12 col-lg-8">
      <h3 class='sr-only' id='sr-footer-heading'>Footer navigation</h3>
      <ul class="list-style-none d-flex flex-wrap col-12 flex-justify-center flex-lg-justify-between mb-2 mb-lg-0" aria-labelledby='sr-footer-heading'>
          <li class="mr-3 mr-lg-0"><a href="https://docs.github.com/en/github/site-policy/github-terms-of-service" data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to terms&quot;,&quot;label&quot;:&quot;text:terms&quot;}">Terms</a></li>
          <li class="mr-3 mr-lg-0"><a href="https://docs.github.com/en/github/site-policy/github-privacy-statement" data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to privacy&quot;,&quot;label&quot;:&quot;text:privacy&quot;}">Privacy</a></li>
          <li class="mr-3 mr-lg-0"><a data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to security&quot;,&quot;label&quot;:&quot;text:security&quot;}" href="https://github.com/security">Security</a></li>
          <li class="mr-3 mr-lg-0"><a href="https://www.githubstatus.com/" data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to status&quot;,&quot;label&quot;:&quot;text:status&quot;}">Status</a></li>
          <li class="mr-3 mr-lg-0"><a data-ga-click="Footer, go to help, text:Docs" href="https://docs.github.com">Docs</a></li>
          <li class="mr-3 mr-lg-0"><a href="https://support.github.com?tags=dotcom-footer" data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to contact&quot;,&quot;label&quot;:&quot;text:contact&quot;}">Contact GitHub</a></li>
          <li class="mr-3 mr-lg-0"><a href="https://github.com/pricing" data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to Pricing&quot;,&quot;label&quot;:&quot;text:Pricing&quot;}">Pricing</a></li>
        <li class="mr-3 mr-lg-0"><a href="https://docs.github.com" data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to api&quot;,&quot;label&quot;:&quot;text:api&quot;}">API</a></li>
        <li class="mr-3 mr-lg-0"><a href="https://services.github.com" data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to training&quot;,&quot;label&quot;:&quot;text:training&quot;}">Training</a></li>
          <li class="mr-3 mr-lg-0"><a href="https://github.blog" data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to blog&quot;,&quot;label&quot;:&quot;text:blog&quot;}">Blog</a></li>
          <li><a data-ga-click="Footer, go to about, text:about" href="https://github.com/about">About</a></li>
      </ul>
    </nav>
  </div>

  <div class="d-flex flex-justify-center pb-6">
    <span class="f6 color-fg-muted"></span>
  </div>
</footer>




  <div id="ajax-error-message" class="ajax-error-message flash flash-error" hidden>
    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-alert">
    <path fill-rule="evenodd" d="M8.22 1.754a.25.25 0 00-.44 0L1.698 13.132a.25.25 0 00.22.368h12.164a.25.25 0 00.22-.368L8.22 1.754zm-1.763-.707c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0114.082 15H1.918a1.75 1.75 0 01-1.543-2.575L6.457 1.047zM9 11a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.25a.75.75 0 00-1.5 0v2.5a.75.75 0 001.5 0v-2.5z"></path>
</svg>
    <button type="button" class="flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path>
</svg>
    </button>
    You can’t perform that action at this time.
  </div>

  <div class="js-stale-session-flash flash flash-warn flash-banner" hidden
    >
    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-alert">
    <path fill-rule="evenodd" d="M8.22 1.754a.25.25 0 00-.44 0L1.698 13.132a.25.25 0 00.22.368h12.164a.25.25 0 00.22-.368L8.22 1.754zm-1.763-.707c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0114.082 15H1.918a1.75 1.75 0 01-1.543-2.575L6.457 1.047zM9 11a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.25a.75.75 0 00-1.5 0v2.5a.75.75 0 001.5 0v-2.5z"></path>
</svg>
    <span class="js-stale-session-flash-signed-in" hidden>You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
    <span class="js-stale-session-flash-signed-out" hidden>You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
  </div>
    <template id="site-details-dialog">
  <details class="details-reset details-overlay details-overlay-dark lh-default color-fg-default hx_rsm" open>
    <summary role="button" aria-label="Close dialog"></summary>
    <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast hx_rsm-dialog hx_rsm-modal">
      <button class="Box-btn-octicon m-0 btn-octicon position-absolute right-0 top-0" type="button" aria-label="Close dialog" data-close-dialog>
        <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path>
</svg>
      </button>
      <div class="octocat-spinner my-6 js-details-dialog-spinner"></div>
    </details-dialog>
  </details>
</template>

    <div class="Popover js-hovercard-content position-absolute" style="display: none; outline: none;" tabindex="0">
  <div class="Popover-message Popover-message--bottom-left Popover-message--large Box color-shadow-large" style="width:360px;">
  </div>
</div>

    <template id="snippet-clipboard-copy-button">
  <div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path fill-rule="evenodd" d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 010 1.5h-1.5a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-1.5a.75.75 0 011.5 0v1.5A1.75 1.75 0 019.25 16h-7.5A1.75 1.75 0 010 14.25v-7.5z"></path><path fill-rule="evenodd" d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0114.25 11h-7.5A1.75 1.75 0 015 9.25v-7.5zm1.75-.25a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-7.5a.25.25 0 00-.25-.25h-7.5z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
    </clipboard-copy>
  </div>
</template>


    <style>
      .user-mention[href$="/sean207cc"] {
        color: var(--color-user-mention-fg);
        background-color: var(--color-user-mention-bg);
        border-radius: 2px;
        margin-left: -2px;
        margin-right: -2px;
        padding: 0 2px;
      }
    </style>


      </div>

      <div id="js-global-screen-reader-notice" class="sr-only" aria-live="polite" ></div>
  </body>
</html>

