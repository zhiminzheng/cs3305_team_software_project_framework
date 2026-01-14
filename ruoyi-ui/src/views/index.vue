<template>
  <div class="app-container home">
    <el-row :gutter="20">
      <el-col :sm="24" :lg="12" style="padding-left: 20px">
        <h2>RuoYi Backend Management Framework</h2>
        <p>
          Always wanted to create a backend management system, looked at many excellent open source projects but found none suitable. So I started writing my own backend system in my spare time. This is how RuoYi Management System came about. It can be used for all Web applications, such as website management backend, website member center, CMS, CRM, OA, etc. Of course, you can also deeply customize it to create a stronger system. All frontend and backend code is encapsulated and very concise and easy to use, with low error probability. It also supports mobile client access. The system will continue to update with practical features.
        </p>
        <p>
          <b>Current Version:</b> <span>v{{ version }}</span>
        </p>
        <p>
          <el-tag type="danger">&yen;Free Open Source</el-tag>
        </p>
        <p>
          <el-button
            type="primary"
            size="mini"
            icon="el-icon-cloudy"
            plain
            @click="goTarget('https://gitee.com/y_project/RuoYi-Vue')"
            >Visit Gitee</el-button
          >
          <el-button
            size="mini"
            icon="el-icon-s-home"
            plain
            @click="goTarget('http://ruoyi.vip')"
            >Visit Homepage</el-button
          >
        </p>
      </el-col>

      <el-col :sm="24" :lg="12" style="padding-left: 50px">
        <el-row>
          <el-col :span="12">
            <h2>Technology Stack</h2>
          </el-col>
        </el-row>
        <el-row>
          <el-col :span="6">
            <h4>Backend Technologies</h4>
            <ul>
              <li>SpringBoot</li>
              <li>Spring Security</li>
              <li>JWT</li>
              <li>MyBatis</li>
              <li>Druid</li>
              <li>Fastjson</li>
              <li>...</li>
            </ul>
          </el-col>
          <el-col :span="6">
            <h4>Frontend Technologies</h4>
            <ul>
              <li>Vue</li>
              <li>Vuex</li>
              <li>Element-ui</li>
              <li>Axios</li>
              <li>Sass</li>
              <li>Quill</li>
              <li>...</li>
            </ul>
          </el-col>
        </el-row>
      </el-col>
    </el-row>
    <el-divider />
    <el-row :gutter="20">
      <el-col :xs="24" :sm="24" :md="12" :lg="8">
        <el-card class="update-log">
          <div slot="header" class="clearfix">
            <span>Contact Information</span>
          </div>
          <div class="body">
            <p>
              <i class="el-icon-s-promotion"></i> Official Website: <el-link
                href="http://www.ruoyi.vip"
                target="_blank"
                >http://www.ruoyi.vip</el-link
              >
            </p>
            <p>
              <i class="el-icon-user-solid"></i> QQ Group: <s> Full 937441 </s> <s> Full 887144332 </s>
              <s> Full 180251782 </s> <s> Full 104180207 </s> <s> Full 186866453 </s> <s> Full 201396349 </s>
              <s> Full 101456076 </s> <s> Full 101539465 </s> <s> Full 264312783 </s> <s> Full 167385320 </s> 
              <s> Full 104748341 </s> <s> Full 160110482 </s> <s> Full 170801498 </s> <s> Full 108482800 </s> 
              <s> Full 101046199 </s> <s> Full 136919097 </s> <s> Full 143961921 </s> <s> Full 174951577 </s> 
              <s> Full 161281055 </s> <s> Full 138988063 </s> <s> Full 151450850 </s> <s> Full 224622315 </s>
              <s> Full 287842588 </s> <s> Full 187944233 </s> <s> Full 228578329 </s> <s> Full 191164766 </s>
              <a href="http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=EeCBXu51I1zPWRia2uskpjDRx6VrbnFN&authKey=Xm8yDxk0%2FyYGI11oxhXaQnTn4K7UwCk7Kn2MZTh3P1JxLctollAkyeySjnaILDkb&noverify=0&group_code=174569686" target="_blank">174569686</a>
            </p>
            <p>
              <i class="el-icon-chat-dot-round"></i> WeChat: <a
                href="javascript:;"
                >/ *RuoYi</a
              >
            </p>
            <p>
              <i class="el-icon-money"></i> Alipay: <a
                href="javascript:;"
                class="Alipay Information"
                >/ *RuoYi</a
              >
            </p>
          </div>
        </el-card>
      </el-col>
      <el-col :xs="24" :sm="24" :md="12" :lg="8">
        <el-card class="update-log">
          <div slot="header" class="clearfix">
            <span>Update Log</span>
          </div>
          <el-collapse accordion>
            <el-collapse-item title="v3.9.1 - 2025-12-18">
              <ol>
                <li>Support referer protection function</li>
                <li>Menu navigation settings support pure top</li>
                <li>Use yauaa instead of bitwalker</li>
                <li>Remove old avatar file after user avatar change</li>
                <li>Support Excel export multiple sub-lists of objects</li>
                <li>Upgrade oshi to latest version 6.9.1</li>
                <li>Upgrade druid to latest version 1.2.27</li>
                <li>Upgrade fastjson to latest version 2.0.60</li>
                <li>Upgrade spring-security to 5.7.14</li>
                <li>Upgrade tomcat to latest version 9.0.112</li>
                <li>Upgrade commons.io to latest version 2.21.0</li>
                <li>Add validation prompt for user import</li>
                <li>Display column information supports object format</li>
                <li>Ignore JSON serialization of user password field</li>
                <li>Add SET_TITLE method for web page title setting</li>
                <li>Reduce auto-identify json object whitelist configuration scope</li>
                <li>Change login/register page footer copyright to read from configuration</li>
                <li>Fix issue where user department cannot be modified to empty</li>
                <li>Fix navigation bar offset issue when fixed header is enabled</li>
                <li>Fix error when clearing after selecting between in v3 time control</li>
                <li>Fix error when multiple sheets appear under comboReadDict attribute</li>
                <li>Fix blank issue when switching routes after removing all controls in form builder</li>
                <li>Optimize layout settings display</li>
                <li>Optimize dictionary component value loose matching</li>
                <li>Optimize method for getting dictionary type values</li>
                <li>Optimize zip file name for generated code download</li>
                <li>Optimize log record parameter assembly to improve efficiency</li>
                <li>Optimize import file check title row cannot be empty</li>
                <li>Optimize form builder close tab destroy copy plugin</li>
                <li>Optimize Excel statistical row value cell style display</li>
                <li>Optimize data permission control logic, remove permission restrictions</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.9.0 - 2025-05-28">
              <ol>
                <li>Optimize menu search query page</li>
                <li>Navigation bar displays nickname & settings</li>
                <li>Add route name to menu management</li>
                <li>Add footer copyright information & switch</li>
                <li>Disable role assignment does not allow selection</li>
                <li>Excel import/export supports multiple images</li>
                <li>Add tab icon display switch function</li>
                <li>Upload component adds drag sort attribute</li>
                <li>Show/hide column component supports select all/none</li>
                <li>Initial password supports custom modification strategy</li>
                <li>Account password supports custom update cycle</li>
                <li>Code generation list supports sorting by time</li>
                <li>Support rich text copy paste image upload to url</li>
                <li>Support file & image component custom address & parameters</li>
                <li>Upgrade tomcat to latest version 9.0.105</li>
                <li>Upgrade oshi to latest version 6.8.1</li>
                <li>Upgrade fastjson to latest version 2.0.57</li>
                <li>Upgrade commons.io to latest version 2.19.0</li>
                <li>Remove runjs dependency from package.json</li>
                <li>Remove eslint dependency from package.json</li>
                <li>Remove vue-meta dependency from package.json</li>
                <li>Fix code generation master-detail table validation required field failure issue</li>
                <li>Optimize frontend tree structure performance issues</li>
                <li>Optimize frontend route function code processing</li>
                <li>Optimize file upload component new types</li>
                <li>Optimize top menu search bar for multi-level display</li>
                <li>Optimize file & image upload component add disabled attribute</li>
                <li>Optimize issue where error information cannot be obtained when null pointer exception occurs</li>
                <li>Optimize scheduled task character contains multiple brackets causing data errors</li>
                <li>Optimize login & register page header uses VUE_APP_TITLE configuration value</li>
                <li>Optimize Excel date format export inconsistency after double-click leaving the set format</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.8.9 - 2024-12-30">
              <ol>
                <li>User management supports column dragging</li>
                <li>Modify theme style local reading</li>
                <li>User avatar http(s) link support</li>
                <li>User management filters out disabled departments</li>
                <li>Support custom display Excel attribute columns</li>
                <li>Operation log records DELETE request parameters</li>
                <li>Whitelist supports wildcard path matching</li>
                <li>Check if file name contains special characters</li>
                <li>Code generation create table blocks illegal characters</li>
                <li>Menu breadcrumb navigation supports multi-level display</li>
                <li>Excel annotation supports wrapText whether to allow content wrapping</li>
                <li>Code generation adds configuration whether to allow file overwrite to local</li>
                <li>Fix role disabled permission not invalid issue</li>
                <li>Fix code generation parent menu display issue</li>
                <li>Fix export sub-list object can only be at the end issue</li>
                <li>Fix TopNav cannot correctly get active issue</li>
                <li>Fix default closed Tags-Views internal link page cannot open</li>
                <li>Upgrade oshi to latest version 6.6.5</li>
                <li>Upgrade tomcat to latest version 9.0.96</li>
                <li>Upgrade fastjson to latest version 2.0.53</li>
                <li>Upgrade logback to latest version 1.2.13</li>
                <li>Upgrade spring-framework to latest version 5.3.39</li>
                <li>Upgrade quill to latest version 2.0.2</li>
                <li>Upgrade axios to latest version 0.28.1</li>
                <li>Optimize ID card desensitization regex</li>
                <li>Optimize permission update sync cache</li>
                <li>Optimize query time range date format</li>
                <li>Optimize parameter key value change to multi-line text</li>
                <li>Optimize import file with title close cleanup</li>
                <li>Optimize upload image with domain name does not add prefix</li>
                <li>Optimize special character password modification failure issue</li>
                <li>Optimize no user ID does not check data permission</li>
                <li>Optimize TopNav internal link menu click no highlight</li>
                <li>Optimize menu management switch Mini layout disorder issue</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.8.8 - 2024-06-30">
              <ol>
                <li>Add route name to menu management</li>
                <li>Add data desensitization filter annotation</li>
                <li>User password adds illegal character validation</li>
                <li>Limit user operation data permission scope</li>
                <li>Code generation adds create table structure function</li>
                <li>Reduce scheduled task whitelist configuration scope</li>
                <li>Optimize code generation master-detail table association query method</li>
                <li>Excel annotation adds attribute comboReadDict</li>
                <li>Excel annotation ColumnType type adds text</li>
                <li>Add internationalization resource file configuration</li>
                <li>Upgrade oshi to latest version 6.6.1</li>
                <li>Upgrade druid to latest version 1.2.23</li>
                <li>Upgrade core-js to latest version 3.37.1</li>
                <li>Update User-Agent in HttpUtils</li>
                <li>Update compressionPlugin to 6.1.2 to support node18+</li>
                <li>Upgrade spring-security to security version to prevent vulnerability risks</li>
                <li>Upgrade spring-framework to security version to prevent vulnerability risks</li>
                <li>Optimize custom XSS annotation matching method</li>
                <li>Optimize cache monitoring key name list sort display</li>
                <li>Optimize scheduled task log default sort by time</li>
                <li>Optimize default file size over 2G invalid issue</li>
                <li>Optimize table query special characters use backslash for escaping</li>
                <li>Optimize scheduled task cron expression hour configuration display error issue</li>
                <li>Optimize multiple custom data permissions use in query to avoid multiple concatenations</li>
                <li>Optimize import Excel when setting dictType attribute repeated cache query issue</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.8.7 - 2023-12-08">
              <ol>
                <li>Operation log records department name</li>
                <li>Global data stores user ID</li>
                <li>Add programmatic resource access permission judgment</li>
                <li>Operation log list adds IP address query</li>
                <li>Scheduled task add page removes status option</li>
                <li>Code generation supports selecting frontend template type</li>
                <li>Show/hide column component supports checkbox popup type</li>
                <li>Common sort attribute orderBy parameter limits length</li>
                <li>Excel custom data processor adds cell/workbook objects</li>
                <li>Upgrade oshi to latest version 6.4.8</li>
                <li>Upgrade druid to latest version 1.2.20</li>
                <li>Upgrade fastjson to latest version 2.0.43</li>
                <li>Upgrade pagehelper to latest version 1.4.7</li>
                <li>Upgrade commons.io to latest version 2.13.0</li>
                <li>Upgrade element-ui to latest version 2.15.14</li>
                <li>Fix five-level route cache invalid issue</li>
                <li>Fix external link with port exception</li>
                <li>Fix tree template parent code variable error</li>
                <li>Fix dictionary table detail page search issue</li>
                <li>Fix internal link iframe parameter not passed issue</li>
                <li>Fix custom dictionary style not effective issue</li>
                <li>Fix dictionary cache delete method parameter error issue</li>
                <li>Fix Excel import data temporary file cannot delete issue</li>
                <li>Fix unlogged access with parameters parameter loss after success issue</li>
                <li>Fix HeaderSearch component jump query parameter loss issue</li>
                <li>Fix code generation import required fields do not match database issue</li>
                <li>Fix Excel import cannot get dictType dictionary value issue</li>
                <li>Optimize download zip method adds overlay</li>
                <li>Optimize avatar upload parameter adds file name</li>
                <li>Optimize dictionary tag supports custom separator</li>
                <li>Optimize menu management type button status optional</li>
                <li>Optimize frontend prevent duplicate submission data size limit</li>
                <li>Optimize TopNav menu no icon svg not displayed</li>
                <li>Optimize number amount uppercase conversion precision loss issue</li>
                <li>Optimize rich text Editor component validate image format</li>
                <li>Optimize tab being blocked in Firefox browser issue</li>
                <li>Optimize personal center/basic info modification data display issue</li>
                <li>Optimize cache monitoring chart supports adaptive adjustment with screen size</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.8.6 - 2023-06-30">
              <ol>
                <li>Support login IP blacklist restriction</li>
                <li>Add monitoring page icon display</li>
                <li>Operation log adds cost time attribute</li>
                <li>Block scheduled task bean illegal characters</li>
                <li>Log management uses index to improve query performance</li>
                <li>Log annotation supports excluding specified request parameters</li>
                <li>Support custom hidden attribute column filter sub-objects</li>
                <li>Upgrade oshi to latest version 6.4.3</li>
                <li>Upgrade druid to latest version 1.2.16</li>
                <li>Upgrade fastjson to latest version 2.0.34</li>
                <li>Upgrade spring-boot to latest version 2.5.15</li>
                <li>Upgrade element-ui to latest version 2.15.13</li>
                <li>Remove apache/commons-fileupload dependency</li>
                <li>Fix layout disorder issue when switching pages</li>
                <li>Fix Anonymous annotation null pointer issue</li>
                <li>Fix internal error message issue when route jump is blocked</li>
                <li>Fix isMatchedIp parameter judgment null pointer issue</li>
                <li>Fix user multi-role data permission possible permission escalation issue</li>
                <li>Fix first-level menu route parameter setting invalid issue after enabling TopNav</li>
                <li>Fix DictTag component value display when no matching value</li>
                <li>Optimize file download exception</li>
                <li>Optimize icon selection component highlight echo</li>
                <li>Optimize navigation bar offset issue after popup</li>
                <li>Optimize password modification log stores plaintext issue</li>
                <li>Optimize tab bar close others exception issue</li>
                <li>Optimize tab close left option excludes home page option</li>
                <li>Optimize close current tab page jump to rightmost tab page</li>
                <li>Optimize cache list clear operation prompt unchanged issue</li>
                <li>Optimize characters without underscore not camel case processing</li>
                <li>Optimize user import update needs to get user ID issue</li>
                <li>Optimize sidebar platform title sync with VUE_APP_TITLE</li>
                <li>Optimize export Excel when setting dictType attribute repeated cache query issue</li>
                <li>Connection pool Druid supports new configuration connectTimeout and socketTimeout</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.8.5 - 2023-01-01">
              <ol>
                <li>Block scheduled task illegal characters</li>
                <li>Cancel department selection when reset</li>
                <li>Add return warning message prompt</li>
                <li>Ignore unnecessary attribute data return</li>
                <li>Remove previous cache configuration when modifying parameter key name</li>
                <li>Validate data permission before importing and updating user data</li>
                <li>Compatible with Excel dropdown content too much cannot display issue</li>
                <li>Upgrade echarts to latest version 5.4.0</li>
                <li>Upgrade core-js to latest version 3.25.3</li>
                <li>Upgrade oshi to latest version 6.4.0</li>
                <li>Upgrade kaptcha to latest version 2.3.3</li>
                <li>Upgrade druid to latest version 1.2.15</li>
                <li>Upgrade fastjson to latest version 2.0.20</li>
                <li>Upgrade pagehelper to latest version 1.4.6</li>
                <li>Optimize popup content too much display incomplete issue</li>
                <li>Optimize swagger-ui static resources use cache</li>
                <li>Enable TopNav no submenu hide sidebar</li>
                <li>Delete fuse invalid option maxPatternLength</li>
                <li>Optimize export object sub-list empty will show [] issue</li>
                <li>Optimize edit avatar transparent part becomes black issue</li>
                <li>Optimize small screen modify avatar interface layout misalignment issue</li>
                <li>Fix code generation checkbox attribute invalid issue</li>
                <li>Fix file upload component format validation issue</li>
                <li>Fix echo data dictionary array exception issue</li>
                <li>Fix sheet exceeds maximum row number exception issue</li>
                <li>Fix Log annotation GET request cannot record parameters issue</li>
                <li>Fix scheduling log click multiple times data unchanged issue</li>
                <li>Fix theme color in Drawer component not loading issue</li>
                <li>Fix file name contains special characters file cannot download issue</li>
                <li>Fix table more button switch theme color not effective issue</li>
                <li>Fix certain environment code generation becomes garbled TXT file issue</li>
                <li>Fix code generation image/file/radio required field cannot validate issue</li>
                <li>Fix certain cases user edit dialog role and department cannot modify issue</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.8.4 - 2022-09-26">
              <ol>
                <li>Data logical delete does not perform unique validation</li>
                <li>Excel annotation supports exporting object sub-list methods</li>
                <li>Excel annotation supports custom hidden attribute columns</li>
                <li>Excel annotation supports backgroundColor attribute to set background color</li>
                <li>Support configure password maximum error count/lock time</li>
                <li>Login log adds unlock account function</li>
                <li>Common download method adds config configuration option</li>
                <li>Support multiple permission character matching role data permissions</li>
                <li>Page embedded iframe switch tab does not refresh data</li>
                <li>Operation log records support excluding sensitive attribute fields</li>
                <li>Fix multi-file upload error exception issue</li>
                <li>Fix image preview component src attribute null value console error issue</li>
                <li>Upgrade oshi to latest version 6.2.2</li>
                <li>Upgrade fastjson to latest version 2.0.14</li>
                <li>Upgrade pagehelper to latest version 1.4.3</li>
                <li>Upgrade core-js to latest version 3.25.2</li>
                <li>Upgrade element-ui to latest version 2.15.10</li>
                <li>Optimize task expired does not execute scheduling</li>
                <li>Optimize dictionary data uses store access</li>
                <li>Optimize modify profile avatar being overwritten issue</li>
                <li>Optimize modify user login account duplicate validation</li>
                <li>Optimize code generation sync value NULL issue</li>
                <li>Optimize scheduled task supports executing parent class methods</li>
                <li>Optimize user personal info interface prevents modifying department</li>
                <li>Optimize layout settings uses el-drawer drawer display</li>
                <li>Optimize users without permission edit department missing data</li>
                <li>Optimize log annotation record limits request address length</li>
                <li>Optimize excel/scale attribute export cell numeric type</li>
                <li>Optimize log operation reset button duplicate query issue</li>
                <li>Optimize multiple same role data causes permission SQL duplicate issue</li>
                <li>Optimize table right toolbar (search button show/hide & right style protrusion)</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.8.3 - 2022-06-27">
              <ol>
                <li>Add cache list menu function</li>
                <li>Code generation tree table adds (expand/collapse)</li>
                <li>Excel annotation supports color font color</li>
                <li>Add Anonymous annotation for anonymous access without authentication</li>
                <li>User avatar upload limited to image format only</li>
                <li>Interface uses generics to see response attribute fields</li>
                <li>Check if scheduled task bean package name is whitelist configuration</li>
                <li>Add tab openPage supports passing parameters</li>
                <li>User cache info adds department ancestors list</li>
                <li>Upgrade element-ui to latest version 2.15.8</li>
                <li>Upgrade oshi to latest version 6.1.6</li>
                <li>Upgrade druid to latest version 1.2.11</li>
                <li>Upgrade fastjson to latest version 2.0.8</li>
                <li>Upgrade spring-boot to latest version 2.5.14</li>
                <li>Downgrade jsencrypt version to support IE browser</li>
                <li>Delete redundant salt field</li>
                <li>Add method to get file name without suffix</li>
                <li>Add method to get attribute value from configuration file</li>
                <li>Add content encoding/decoding for plugin integration</li>
                <li>Dictionary type must start with letter, and can only be (lowercase letters, numbers, underscore)</li>
                <li>Optimize set pagination parameter default value</li>
                <li>Optimize filter empty string parameter processing</li>
                <li>Optimize display order orderNum type to integer</li>
                <li>Optimize form builder button does not display regex validation</li>
                <li>Optimize dictionary data echo style dropdown display value</li>
                <li>Optimize R response success status code consistent with global</li>
                <li>Optimize druid enable wall filter exception issue</li>
                <li>Optimize user management left tree component adds selected highlight keep</li>
                <li>Optimize add user with role info & user with post info logic</li>
                <li>Optimize default not enable compressed file cache to prevent node_modules too large</li>
                <li>Fix dictionary data display incomplete issue</li>
                <li>Fix operation log query type condition 0 will query all data issue</li>
                <li>Fix Excel annotation prompt/combo used together not effective issue</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.8.2 - 2022-04-01">
              <ol>
                <li>Frontend supports setting whether to prevent duplicate data submission</li>
                <li>Enable TopNav no submenu case hide sidebar</li>
                <li>Sidebar menu name too long hover display title</li>
                <li>User access control validates data permissions to prevent privilege escalation</li>
                <li>Export Excel blocks formulas to prevent CSV injection risk</li>
                <li>Component ImagePreview supports multi-image preview display</li>
                <li>Component ImageUpload supports multiple images simultaneous selection upload</li>
                <li>Component FileUpload supports multiple files simultaneous selection upload</li>
                <li>Service monitoring adds runtime parameter information display</li>
                <li>Scheduled task target string filters special characters</li>
                <li>Scheduled task target string validates package name whitelist</li>
                <li>Code generation list images support preview</li>
                <li>Code generation edit modify opens new tab</li>
                <li>Code generation adds Java type Boolean</li>
                <li>Code generation sub-table supports date/dictionary configuration</li>
                <li>Code generation sync preserves required/type options</li>
                <li>Upgrade oshi to latest version 6.1.2</li>
                <li>Upgrade fastjson to latest version 1.2.80</li>
                <li>Upgrade pagehelper to latest version 1.4.1</li>
                <li>Upgrade spring-boot to latest version 2.5.11</li>
                <li>Upgrade spring-boot-mybatis to latest version 2.2.2</li>
                <li>Add missing pagination parameter rationalization attribute</li>
                <li>Modify npm about to expire registry source address</li>
                <li>Fix pagination component requests twice issue</li>
                <li>Fix common file download interface CORS issue</li>
                <li>Fix Xss annotation field value empty exception issue</li>
                <li>Fix tab right-click refresh loses parameters issue</li>
                <li>Fix form clear element position not vertically centered issue</li>
                <li>Fix service monitoring runtime parameter display condition error</li>
                <li>Fix import Excel dictionary field type Long escape to empty issue</li>
                <li>Fix login timeout refresh page jump to login page still prompts re-login issue</li>
                <li>Optimize load dictionary cache data</li>
                <li>Optimize IP address gets multiple issue</li>
                <li>Optimize task queue full task rejection strategy</li>
                <li>Optimize file upload compatible with Weblogic environment</li>
                <li>Optimize scheduled task default save to memory execution</li>
                <li>Optimize department modify zoom misalignment issue</li>
                <li>Optimize Excel format different types of date objects</li>
                <li>Optimize menu table keyword causes plugin error issue</li>
                <li>Optimize Oracle user avatar column empty not display issue</li>
                <li>Optimize page if no matching dictionary label returns original dictionary value</li>
                <li>Optimize fix login expired multiple requests prompt multiple popups issue</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.8.1 - 2022-01-01">
              <ol>
                <li>Add Vue3 frontend code generation template</li>
                <li>Add image preview component</li>
                <li>Add compression plugin implements Gzip packaging</li>
                <li>Custom xss validation annotation implementation</li>
                <li>Custom text copy paste directive</li>
                <li>Code generation preview supports copy content</li>
                <li>Route supports separate configuration menu or role permissions</li>
                <li>User management department query select node pagination parameter initialization</li>
                <li>Fix user assign role attribute error</li>
                <li>Fix packaged font icon occasional garbled issue</li>
                <li>Fix menu management reset form error</li>
                <li>Fix version difference causes lazy loading error issue</li>
                <li>Fix Cron component week echo issue</li>
                <li>Fix scheduled task multiple parameters comma separated issue</li>
                <li>Fix query list by ID possible primary key overflow issue</li>
                <li>Fix tomcat configuration parameter expired issue</li>
                <li>Upgrade clipboard to latest version 2.0.8</li>
                <li>Upgrade oshi to latest version v5.8.6</li>
                <li>Upgrade fastjson to latest version 1.2.79</li>
                <li>Upgrade spring-boot to latest version 2.5.8</li>
                <li>Upgrade log4j2 to 2.17.1 to prevent vulnerability risk</li>
                <li>Optimize download parse blob exception prompt</li>
                <li>Optimize code generation dictionary group duplicate issue</li>
                <li>Optimize query user role group & post group code</li>
                <li>Optimize scheduled task cron expression hour setting 24</li>
                <li>Optimize user import prompt overflow shows scrollbar</li>
                <li>Optimize prevent duplicate submission identifier combination (key+url+header)</li>
                <li>Optimize pagination method set to common convenient flexible call</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.8.0 - 2021-12-01">
              <ol>
                <li>Add matching and synchronized Vue3 frontend version</li>
                <li>Add common methods to simplify modal/cache/download/permission/tab usage</li>
                <li>Optimize export data/use common download method</li>
                <li>Excel annotation supports custom data processor</li>
                <li>Excel annotation supports import/export title information</li>
                <li>Excel import supports @Excels annotation</li>
                <li>Add component data-dict to simplify dictionary usage</li>
                <li>Add Jaxb dependency to prevent compatibility errors in jdk8+</li>
                <li>Production environment uses route lazy loading to improve page response speed</li>
                <li>Fix five-level menu 404 issue</li>
                <li>Prevent duplicate submission annotation supports configuring interval time/prompt message</li>
                <li>Log annotation adds whether to save response parameters</li>
                <li>Task blocks illegal characters & parameters ignore commas in double quotes</li>
                <li>Upgrade SpringBoot to latest version 2.5.6</li>
                <li>Upgrade pagehelper to latest version 1.4.0</li>
                <li>Upgrade spring-boot-mybatis to latest version 2.2.0</li>
                <li>Upgrade oshi to latest version v5.8.2</li>
                <li>Upgrade druid to latest version 1.2.8</li>
                <li>Upgrade velocity to latest version 2.3</li>
                <li>Upgrade fastjson to latest version 1.2.78</li>
                <li>Upgrade axios to latest version 0.24.0</li>
                <li>Upgrade dart-sass to version 1.32.13</li>
                <li>Upgrade core-js to latest version 3.19.1</li>
                <li>Upgrade jsencrypt to latest version 3.2.1</li>
                <li>Upgrade js-cookie to latest version 3.0.1</li>
                <li>Upgrade file-saver to latest version 2.0.5</li>
                <li>Upgrade sass-loader to latest version 10.1.1</li>
                <li>Upgrade element-ui to latest version 2.15.6</li>
                <li>Add sendGet no-parameter request method</li>
                <li>Disable el-tag component gradient animation</li>
                <li>Code generation click preview reset active tab</li>
                <li>AjaxResult rewrite put method for convenient chaining</li>
                <li>Optimize login/captcha request headers do not set token</li>
                <li>Optimize user personal info interface prevents modifying username</li>
                <li>Optimize Cron expression generator destroy on close to avoid cache</li>
                <li>Optimize registration success prompt message type success</li>
                <li>Optimize aop syntax, use spring auto-injection annotation</li>
                <li>Optimize record login info, remove unnecessary modifications</li>
                <li>Optimize mybatis global default executor</li>
                <li>Optimize Excel import image possible exceptions</li>
                <li>Fix code generation template master-detail table delete missing transaction</li>
                <li>Fix log record possible conversion exception</li>
                <li>Fix code generation checkbox dictionary missing issue</li>
                <li>Fix closing xss function causes RepeatableFilter failure</li>
                <li>Fix string cannot be unescaped issue</li>
                <li>Fix backend master-detail table code template method name generation error</li>
                <li>Fix xss filter format exception</li>
                <li>Fix swagger not specifying dataTypeClass causes startup warn log</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.7.0 - 2021-09-13">
              <ol>
                <li>Parameter management supports configuring captcha switch</li>
                <li>Add whether to enable user registration function</li>
                <li>Scheduled task supports online cron expression generation</li>
                <li>Menu management supports configuring route parameters</li>
                <li>Support custom annotation implements interface rate limiting</li>
                <li>Excel annotation supports Image import</li>
                <li>Custom popup overflow scroll style</li>
                <li>Custom draggable popup width directive</li>
                <li>Custom draggable popup height directive</li>
                <li>Fix arbitrary account privilege escalation issue</li>
                <li>Check user data permission scope when modifying</li>
                <li>Fix save configuration theme color failure issue</li>
                <li>Add dark menu style theme</li>
                <li>Menu & department add expand/collapse function</li>
                <li>Tab adds close left & add icon</li>
                <li>Top menu excludes hidden default routes</li>
                <li>Top menu syncs system theme style</li>
                <li>Jump route highlights corresponding menu bar</li>
                <li>Code generation master-detail table multi-select row data</li>
                <li>Date range supports adding multiple groups</li>
                <li>Upgrade element-ui to latest version 2.15.5</li>
                <li>Upgrade oshi to latest version v5.8.0</li>
                <li>Upgrade commons.io to latest version v2.11.0</li>
                <li>Scheduled task blocks ldap remote call</li>
                <li>Scheduled task blocks http(s) remote call</li>
                <li>Supplement scheduled task table field comments</li>
                <li>Scheduled task transaction rollback for check exceptions</li>
                <li>Enable parent department status excludes top node</li>
                <li>Rich text adds upload file size limit</li>
                <li>Default homepage uses keep-alive cache</li>
                <li>Modify code generation dictionary echo style</li>
                <li>Custom pagination rationalization input parameters</li>
                <li>Fix dictionary component value integer not display issue</li>
                <li>Fix scheduled task log execution status display</li>
                <li>Role & menu add field attribute prompt information</li>
                <li>Fix role assign user page parameter type error reminder</li>
                <li>Optimize layout settings animation effects</li>
                <li>Optimize exception handling information</li>
                <li>Optimize error token causes parsing exception</li>
                <li>Password box adds display toggle password icon</li>
                <li>Scheduled task adds more operations</li>
                <li>More operations button adds permission control</li>
                <li>Import user style optimization</li>
                <li>Extract common methods to base controller</li>
                <li>Optimize use permission tool to get user information</li>
                <li>Optimize user cannot delete themselves</li>
                <li>Optimize XSS cross-site scripting filter</li>
                <li>Optimize code generation template</li>
                <li>Captcha default 20s timeout</li>
                <li>Clear URL object reference when BLOB download</li>
                <li>Code generation import table sorted by creation time</li>
                <li>Fix code generation page data edit save always jump to first page issue</li>
                <li>Fix Safari browser cannot format utc date format yyyy-MM-dd'T'HH:mm:ss.SSS issue</li>
                <li>Multi-image upload component removes redundant api address & validation failure causes image deletion issue & cannot delete corresponding image fix</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.6.0 - 2021-07-12">
              <ol>
                <li>Role management adds assign user function</li>
                <li>User management adds assign role function</li>
                <li>Log list supports sort operation</li>
                <li>Optimize parameter & dictionary cache operation</li>
                <li>System layout configuration supports dynamic title switch</li>
                <li>Menu route configuration supports internal link access</li>
                <li>Default access backend homepage adds prompt message</li>
                <li>Rich text default upload returns url type</li>
                <li>Add custom popup drag directive</li>
                <li>Global register common components</li>
                <li>Global mount dictionary tag component</li>
                <li>ImageUpload component supports multiple image upload</li>
                <li>FileUpload component supports multiple file upload</li>
                <li>File upload component adds quantity limit attribute</li>
                <li>Rich text editor component adds type attribute</li>
                <li>Rich text component toolbar configures video</li>
                <li>Package common iframe component</li>
                <li>Restrict super administrator not allowed to operate</li>
                <li>User information length validation limit</li>
                <li>Pagination component adds pagerCount attribute</li>
                <li>Add bat script execution application</li>
                <li>Upgrade oshi to latest version v5.7.4</li>
                <li>Upgrade element-ui to latest version 2.15.2</li>
                <li>Upgrade pagehelper to latest version 1.3.1</li>
                <li>Upgrade commons.io to latest version v2.10.0</li>
                <li>Upgrade commons.fileupload to latest version v1.4</li>
                <li>Upgrade swagger to latest version v3.0.0</li>
                <li>Fix close confirm prompt box console error issue</li>
                <li>Fix existing SQL injection vulnerability issue</li>
                <li>Scheduled task blocks rmi remote call</li>
                <li>Fix user search pagination variable error</li>
                <li>Fix export role data scope translation missing only self</li>
                <li>Fix form builder select dropdown console error issue</li>
                <li>Optimize image tool class read file</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.5.0 - 2021-05-25">
              <ol>
                <li>Add menu navigation display style TopNav (false for left navigation menu, true for top navigation menu)</li>
                <li>Layout settings support save & reset configuration</li>
                <li>Fix tree table data display incomplete & slow loading issue</li>
                <li>Add IE browser version too low prompt page</li>
                <li>Record last login IP & time after user login</li>
                <li>Add overlay after page export button click</li>
                <li>Rich text editor supports custom upload address</li>
                <li>Rich text editor component adds readOnly attribute</li>
                <li>Tab TagsView adds close right function</li>
                <li>Show/hide column component loads initial default hidden columns</li>
                <li>Close avatar upload window restore default image</li>
                <li>Personal info adds phone & email duplicate validation</li>
                <li>Code generation template export button adds overlay after click</li>
                <li>Code generation template tree table operation column adds add button</li>
                <li>Code generation template fixes master-detail table field duplicate name issue</li>
                <li>Upgrade fastjson to latest version 1.2.76</li>
                <li>Upgrade druid to latest version v1.2.6</li>
                <li>Upgrade mybatis to latest version 3.5.6 to prevent remote code execution vulnerability</li>
                <li>Upgrade oshi to latest version v5.6.0</li>
                <li>Velocity removes commons-collections version to prevent 3.2.1 version deserialization vulnerability</li>
                <li>Data monitoring page default account password prevents privilege escalation access</li>
                <li>Fix Firefox form builder drag opens new tab issue</li>
                <li>Fix backend import table permission identifier</li>
                <li>Fix frontend operation log & login log permission identifier</li>
                <li>Set Redis configuration HashKey serialization</li>
                <li>Delete operation log record information</li>
                <li>Upload media type adds video format</li>
                <li>Fix request parameter not passed record log exception issue</li>
                <li>Optimize xss validation json request condition</li>
                <li>Tree structure update child node uses replaceFirst</li>
                <li>Optimize ExcelUtil null value processing</li>
                <li>Log record filters BindingResult object to prevent exception</li>
                <li>Fix mini type button invalid issue after modifying theme</li>
                <li>Optimize common download delete node after completion</li>
                <li>Common Controller adds response return message</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.4.0 - 2021-02-22">
              <ol>
                <li>Code generation template supports master-detail table</li>
                <li>Table right toolbar component supports show/hide columns</li>
                <li>Image component adds preview & remove function</li>
                <li>Excel annotation supports Image export</li>
                <li>Operation button group adjusts to plain button style</li>
                <li>Code generation supports file upload component</li>
                <li>Code generation date control distinguishes range</li>
                <li>Code generation database text type generates form textarea</li>
                <li>User phone email & menu component modification allows empty string</li>
                <li>Upgrade SpringBoot to latest version 2.2.13 to improve startup speed</li>
                <li>Upgrade druid to latest version v1.2.4</li>
                <li>Upgrade fastjson to latest version 1.2.75</li>
                <li>Upgrade element-ui to latest version 2.15.0</li>
                <li>Fix IE11 browser error issue</li>
                <li>Optimize multi-level menu switching cannot cache issue</li>
                <li>Fix four-level menu cannot display issue</li>
                <li>Fix sidebar static route loss issue</li>
                <li>Fix role management-edit role-function permission display exception</li>
                <li>Configuration file adds redis database index attribute</li>
                <li>Permission tool class adds admin judgment</li>
                <li>Role non-custom permission scope clears selected value</li>
                <li>Fix import data negative float precision loss issue</li>
                <li>Remove path-to-regexp regex matching plugin</li>
                <li>Fix generate tree table code exception</li>
                <li>Modify ip field length to prevent ipv6 address length insufficient</li>
                <li>Prevent get request parameter value false or 0 special values causes incorrect parameter passing</li>
                <li>Login push adds catch to prevent check error</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.3.0 - 2020-12-14">
              <ol>
                <li>Add cache monitoring function</li>
                <li>Support theme style configuration</li>
                <li>Fix multi-level menu switching cannot cache issue</li>
                <li>Multi-level menu auto-configure component</li>
                <li>Code generation preview supports highlight display</li>
                <li>Support Get request mapping Params parameters</li>
                <li>Delete user and role unbind association</li>
                <li>Remove user phone email department required validation</li>
                <li>Excel supports annotation align alignment</li>
                <li>Excel supports importing Boolean type data</li>
                <li>Optimize avatar style, mouse hover overlay</li>
                <li>Code generation preview provides scroll mechanism</li>
                <li>Code generation removes redundant number float type</li>
                <li>Fix convert string target character set attribute</li>
                <li>Echo data dictionary prevents null value error</li>
                <li>Log record adds filter multi-file scenario</li>
                <li>Fix cache Set method may cause nesting issue</li>
                <li>Remove some redundant frontend dependencies</li>
                <li>Prevent security scan YUI risk prompt</li>
                <li>Modify node-sass to dart-sass</li>
                <li>Upgrade SpringBoot to latest version 2.1.18</li>
                <li>Upgrade poi to latest version 4.1.2</li>
                <li>Upgrade oshi to latest version v5.3.6</li>
                <li>Upgrade bitwalker to latest version 1.21</li>
                <li>Upgrade axios to latest version 0.21.0</li>
                <li>Upgrade element-ui to latest version 2.14.1</li>
                <li>Upgrade vue to latest version 2.6.12</li>
                <li>Upgrade vuex to latest version 3.6.0</li>
                <li>Upgrade vue-cli to version 4.5.9</li>
                <li>Upgrade vue-router to latest version 3.4.9</li>
                <li>Upgrade vue-cli to latest version 4.4.6</li>
                <li>Upgrade vue-cropper to latest version 0.5.5</li>
                <li>Upgrade clipboard to latest version 2.0.6</li>
                <li>Upgrade core-js to latest version 3.8.1</li>
                <li>Upgrade echarts to latest version 4.9.0</li>
                <li>Upgrade file-saver to latest version 2.0.4</li>
                <li>Upgrade fuse.js to latest version 6.4.3</li>
                <li>Upgrade js-beautify to latest version 1.13.0</li>
                <li>Upgrade js-cookie to latest version 2.2.1</li>
                <li>Upgrade path-to-regexp to latest version 6.2.0</li>
                <li>Upgrade quill to latest version 1.3.7</li>
                <li>Upgrade screenfull to latest version 5.0.2</li>
                <li>Upgrade sortablejs to latest version 1.10.2</li>
                <li>Upgrade vuedraggable to latest version 2.24.3</li>
                <li>Upgrade chalk to latest version 4.1.0</li>
                <li>Upgrade eslint to latest version 7.15.0</li>
                <li>Upgrade eslint-plugin-vue to latest version 7.2.0</li>
                <li>Upgrade lint-staged to latest version 10.5.3</li>
                <li>Upgrade runjs to latest version 4.4.2</li>
                <li>Upgrade sass-loader to latest version 10.1.0</li>
                <li>Upgrade script-ext-html-webpack-plugin to latest version 2.1.5</li>
                <li>Upgrade svg-sprite-loader to latest version 5.1.1</li>
                <li>Upgrade vue-template-compiler to latest version 2.6.12</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.2.1 - 2020-11-18">
              <ol>
                <li>Prevent arbitrary file download vulnerability</li>
                <li>Code generation supports upload control</li>
                <li>Add image upload component</li>
                <li>Adjust default homepage</li>
                <li>Upgrade druid to latest version v1.2.2</li>
                <li>mapperLocations configuration supports separator</li>
                <li>Permission information adjustment</li>
                <li>Adjust sql default time</li>
                <li>Fix code generation missing bit type issue</li>
                <li>Upgrade pagehelper to latest version 1.3.0</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v3.2.0 - 2020-10-10">
              <ol>
                <li>Upgrade springboot version to 2.1.17 to improve security</li>
                <li>Upgrade oshi to latest version v5.2.5</li>
                <li>Upgrade druid to latest version v1.2.1</li>
                <li>Upgrade jjwt to version 0.9.1</li>
                <li>Upgrade fastjson to latest version 1.2.74</li>
                <li>Modify sass to node-sass to avoid el-icon icon garbled</li>
                <li>Code generation supports sync database</li>
                <li>Code generation supports rich text control</li>
                <li>Code generation page does not ignore remark attribute</li>
                <li>Code generation adds select required option</li>
                <li>Excel export type NUMERIC supports precision float type</li>
                <li>Excel export targetAttr optimizes value retrieval to prevent get method non-standard</li>
                <li>Excel annotation supports automatic statistics sum</li>
                <li>Excel annotation supports setting BigDecimal precision & rounding rules</li>
                <li>Menu & data permission adds (expand/collapse select all/none parent-child linkage)</li>
                <li>Allow user assigned to department parent node</li>
                <li>Menu adds whether to cache keep-alive</li>
                <li>Table operation column spacing adjustment</li>
                <li>Restrict system built-in parameters not allowed to delete</li>
                <li>Rich text component optimization, supports custom height & image conflict issue</li>
                <li>Rich text toolbar style alignment</li>
                <li>Import excel integer value validation optimization</li>
                <li>Fix tab close all fixed tag route not refresh issue</li>
                <li>Form builder layout component adds button</li>
                <li>Left menu text too long displays ellipsis</li>
                <li>Fix root node as sub-department tree structure display issue</li>
                <li>Fix invoke target string maximum length</li>
                <li>Fix menu prompt information error</li>
                <li>Fix scheduled task execute once permission identifier</li>
                <li>Fix database string type nvarchar</li>
                <li>Optimize recursive child nodes</li>
                <li>Optimize data permission judgment</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>

            <el-collapse-item title="v3.1.0 - 2020-08-13">
              <ol>
                <li>Table toolbar right adds refresh & show/hide query component</li>
                <li>Backend supports CORS cross-domain requests</li>
                <li>Code generation supports selecting parent menu</li>
                <li>Code generation supports custom path</li>
                <li>Code generation supports checkbox</li>
                <li>Excel export/import supports dictType dictionary type</li>
                <li>Excel supports splitting string group content</li>
                <li>Captcha type supports (array calculation, character validation)</li>
                <li>Upgrade vue-cli version to 4.4.4</li>
                <li>Modify node-sass to dart-sass</li>
                <li>Form type Integer/Long sets integer default value</li>
                <li>Code generator default mapper path inconsistent with default mapperScan path</li>
                <li>Optimize prevent duplicate submission interceptor</li>
                <li>Optimize parent menu cannot select itself</li>
                <li>Fix role permission assignment not effective in real-time issue</li>
                <li>Fix online user log record type</li>
                <li>Fix rich text space and indent not effective after save issue</li>
                <li>Fix online user judgment logic</li>
                <li>Unique constraint condition only returns single data</li>
                <li>Add method to get current environment configuration</li>
                <li>Timeout login page jumps to homepage</li>
                <li>Global exception status localization interception handling</li>
                <li>HTML filter changes to escape html</li>
                <li>Check character supports decimal point & downgrade to exception reminder</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>

            <el-collapse-item title="v3.0.0 - 2020-07-20">
              <ol>
                <li>Single application adjusted to multi-module project</li>
                <li>Upgrade element-ui version to 2.13.2</li>
                <li>Delete babel to improve compilation speed</li>
                <li>Add menu default main category</li>
                <li>Encode file name changed to uuid method</li>
                <li>Scheduled task cron expression validation</li>
                <li>Fix role permission modification existing permissions not auto-selected exception</li>
                <li>Prevent switching permission user login 404 issue</li>
                <li>Excel supports sort export sorting</li>
                <li>Create user not allowed to select super administrator role</li>
                <li>Fix code generation import table structure exception page no reminder issue</li>
                <li>Fix code generation click multiple times table modify data unchanged issue</li>
                <li>Fix avatar upload success second open cannot change crop box size and position issue</li>
                <li>Fix layout small or mini user form display misalignment issue</li>
                <li>Fix hot deployment causes strong change exception issue</li>
                <li>Modify user management checkbox width to prevent some browsers showing ellipsis</li>
                <li>IpUtils tool clears Xss special characters to prevent Xff injection attack</li>
                <li>Generate domain if float type uniformly use BigDecimal</li>
                <li>Scheduled task adjusts label-width to prevent deployment misalignment</li>
                <li>Adjust table header fixed column default style</li>
                <li>Code generation template adjustment, field is String and required then add empty string condition</li>
                <li>Code generation dictionary Integer/Long uses parseInt</li>
                <li>
                  Fix dict_sort cannot update to 0 issue & query return adds dict_sort ascending sort
                </li>
                <li>Fix post export permission annotation</li>
                <li>Prohibit encrypted ciphertext return to frontend</li>
                <li>Fix code generation page query condition creation time not effective issue</li>
                <li>Fix homepage search menu external link cannot click jump issue</li>
                <li>Fix menu management select icon, backspace delete does not filter data</li>
                <li>User management department branch node cannot check & display count</li>
                <li>Data scope filter attribute adjustment</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>

            <el-collapse-item title="v2.3.0 - 2020-06-01">
              <ol>
                <li>Upgrade fastjson to latest version 1.2.70 to fix high-risk security vulnerability</li>
                <li>dev startup default opens browser</li>
                <li>vue-cli uses default source-map</li>
                <li>slidebar eslint error optimization</li>
                <li>When tags-view scrolls close right-click menu</li>
                <li>Dictionary management adds cache read</li>
                <li>Parameter management supports cache operation</li>
                <li>Support first-level menu (same level as homepage) display in main area</li>
                <li>Restrict external link address must start with http(s)</li>
                <li>tagview & sidebar theme color syncs with element ui (global)</li>
                <li>Modify data source type priority, first by method, then by class</li>
                <li>Support whether to set token attribute, custom return code message</li>
                <li>swagger request prefix added to configuration</li>
                <li>Login location setting content too long then hide display</li>
                <li>Fix scheduled task execute once button no prompt message issue</li>
                <li>Modify parent department (selection excludes itself and subordinates)</li>
                <li>Common http send method adds parameter contentType encoding type</li>
                <li>Replace IP address query interface</li>
                <li>Fix tab variable undefined</li>
                <li>Add validation department contains non-disabled sub-departments</li>
                <li>Fix scheduled task detail next execution time date display error</li>
                <li>Role management query sets default sort field</li>
                <li>swagger adds enable parameter to control whether to enable</li>
                <li>Only build repeatable read inputStream request for json type requests</li>
                <li>Fix code generation dictionary field int type not auto-selected issue</li>
                <li>vuex username value correction</li>
                <li>Table tree template removes redundant )</li>
                <li>Code generation sequence number correction</li>
                <li>Full screen does not adjust top margin</li>
                <li>Code generation Date field adds default format</li>
                <li>User management role selection permission control</li>
                <li>Fix route lazy loading error issue</li>
                <li>Template sql.vm adds menu status</li>
                <li>Set user name cannot be modified</li>
                <li>dialog adds append-to-body attribute to prevent ie overlay</li>
                <li>Menu distinguishes status and show/hide function</li>
                <li>Upgrade fastjson to latest version 1.2.68 to fix security hardening</li>
                <li>Fix code generation if select dictionary type missing comma issue</li>
                <li>Login request params changed to data to prevent exposing url</li>
                <li>Log return time format processing</li>
                <li>Add handle to control draggable elements</li>
                <li>Layout settings click expands range</li>
                <li>Code generation column attribute sort query</li>
                <li>Code generation column supports drag sort</li>
                <li>Fix time format does not support ios issue</li>
                <li>Form builder adds parent class to prevent conflicts</li>
                <li>Scheduled task concurrent attribute correction</li>
                <li>Role disabled & menu hidden does not query permissions</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>

            <el-collapse-item title="v2.2.0 - 2020-03-18">
              <ol>
                <li>System monitoring adds scheduled task function</li>
                <li>Add a package Web project bat</li>
                <li>Fix tab mouse wheel pressed can close non-closable tag issue</li>
                <li>Fix click logout sometimes no prompt issue</li>
                <li>Fix prevent duplicate submission annotation invalid issue</li>
                <li>Fix notice announcement batch delete exception issue</li>
                <li>Add menu route address required restriction</li>
                <li>Code generation field description editable</li>
                <li>Fix user modify personal info causes cache not expired issue</li>
                <li>Personal info creation time gets correct attribute value</li>
                <li>Operation log detail displays correct type</li>
                <li>Import table click row data selects corresponding checkbox</li>
                <li>Batch replace table prefix logic adjustment</li>
                <li>Fix redirect path expression</li>
                <li>Upgrade element-ui version to 2.13.0</li>
                <li>Operation log sort adjustment</li>
                <li>Fix charts switch sidebar or zoom window display bug</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>

            <el-collapse-item title="v2.1.0 - 2020-02-24">
              <ol>
                <li>Add form builder</li>
                <li>Code generation supports tree table structure</li>
                <li>Add user import</li>
                <li>Fix dynamic load route page refresh issue</li>
                <li>Fix address switch invalid issue</li>
                <li>Localize error prompt page</li>
                <li>Code generation known issues modification</li>
                <li>Fix multi-datasource configuration close exception handling</li>
                <li>Add HTML filter to remove XSS vulnerability risks</li>
                <li>Fix upload avatar console exception</li>
                <li>Fix user management pagination incorrect issue</li>
                <li>Fix captcha record prompt error</li>
                <li>Fix request.js missing Message reference</li>
                <li>Fix table time empty exception</li>
                <li>Add Jackson date deserialization timezone configuration</li>
                <li>Adjust load menu data tree structure based on user permissions</li>
                <li>Adjust successful login does not restore button to prevent multiple clicks</li>
                <li>Modify user personal profile sync cache information</li>
                <li>Fix page el-upload and Editor appear together not display handling</li>
                <li>Fix role management page modify menu permission occasionally not selected issue</li>
                <li>Configuration file adds redis password attribute</li>
                <li>Set mybatis global configuration file</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>

            <el-collapse-item title="v2.0.0 - 2019-12-02">
              <ol>
                <li>Add code generation</li>
                <li>Add @RepeatSubmit annotation to prevent duplicate submission</li>
                <li>Add menu main directory add/delete operation</li>
                <li>Log record filters special objects to prevent conversion exception</li>
                <li>Fix code generation route script error</li>
                <li>User upload avatar real-time sync cache, no need to re-login</li>
                <li>Adjust switch tab does not reload data</li>
                <li>Add jsencrypt implements frontend encryption of parameters</li>
                <li>System exit deletes user cache record</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v1.1.0 - 2019-11-11">
              <ol>
                <li>Add online user management</li>
                <li>Add button group function implementation (batch delete, export, clear)</li>
                <li>Add query condition reset button</li>
                <li>Add Swagger global Token configuration</li>
                <li>Add backend parameter validation</li>
                <li>Fix dictionary management page date query exception</li>
                <li>Modify time function naming to prevent conflicts</li>
                <li>Remove menu parent validation, default to top level</li>
                <li>Fix user password cannot modify issue</li>
                <li>Fix menu type button does not display permission identifier</li>
                <li>Other detail optimizations</li>
              </ol>
            </el-collapse-item>
            <el-collapse-item title="v1.0.0 - 2019-10-08">
              <ol>
                <li>RuoYi frontend-backend separation system officially released</li>
              </ol>
            </el-collapse-item>
          </el-collapse>
        </el-card>
      </el-col>
      <el-col :xs="24" :sm="24" :md="12" :lg="8">
        <el-card class="update-log">
          <div slot="header" class="clearfix">
            <span>Donation Support</span>
          </div>
          <div class="body">
            <img
              src="@/assets/images/pay.png"
              alt="donate"
              width="100%"
            />
            <span style="display: inline-block; height: 30px; line-height: 30px"
              >You can buy the author a coffee to show encouragement</span
            >
          </div>
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: "Index",
  data() {
    return {
      // Version Number
      version: "3.9.1"
    }
  },
  methods: {
    goTarget(href) {
      window.open(href, "_blank")
    }
  }
}
</script>

<style scoped lang="scss">
.home {
  blockquote {
    padding: 10px 20px;
    margin: 0 0 20px;
    font-size: 17.5px;
    border-left: 5px solid #eee;
  }
  hr {
    margin-top: 20px;
    margin-bottom: 20px;
    border: 0;
    border-top: 1px solid #eee;
  }
  .col-item {
    margin-bottom: 20px;
  }

  ul {
    padding: 0;
    margin: 0;
  }

  font-family: "open sans", "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 13px;
  color: #676a6c;
  overflow-x: hidden;

  ul {
    list-style-type: none;
  }

  h4 {
    margin-top: 0px;
  }

  h2 {
    margin-top: 10px;
    font-size: 26px;
    font-weight: 100;
  }

  p {
    margin-top: 10px;

    b {
      font-weight: 700;
    }
  }

  .update-log {
    ol {
      display: block;
      list-style-type: decimal;
      margin-block-start: 1em;
      margin-block-end: 1em;
      margin-inline-start: 0;
      margin-inline-end: 0;
      padding-inline-start: 40px;
    }
  }
}
</style>

