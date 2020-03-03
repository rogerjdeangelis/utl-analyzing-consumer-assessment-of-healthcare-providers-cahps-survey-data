# utl-analyzing-consumer-assessment-of-healthcare-providers-cahps-survey-data
Analyzing consumer assessment of healthcare providers cahps survey data
    Analyzing consumer assessment of healthcare providers CAHPS survey data

    github
    https://tinyurl.com/uhee2uj
    https://github.com/rogerjdeangelis/utl-analyzing-consumer-assessment-of-healthcare-providers-cahps-survey-data

    zip archive
    https://tinyurl.com/trcjk7c
    https://github.com/rogerjdeangelis/utl-analyzing-consumer-assessment-of-healthcare-providers-cahps-survey-data/blob/master/cps.zip

    SAS Forum
    https://tinyurl.com/w34tvp2
    https://communities.sas.com/t5/SAS-Enterprise-Guide/SAS-CAHPS-ANALYSIS-PROGRAM/m-p/629270


    I was able to run the package without errors.
    https://www.ahrq.gov/cahps/surveys-guidance/helpful-resources/analysis/index.html

    *               _   _               _
     _ __ ___   ___| |_| |__   ___   __| |
    | '_ ` _ \ / _ \ __| '_ \ / _ \ / _` |
    | | | | | |  __/ |_| | | | (_) | (_| |
    |_| |_| |_|\___|\__|_| |_|\___/ \__,_|

    ;

    If you unzip the github archive and use root, d:/cps, (or change the root in cc251_mycontrol.sas) then
    you should be able to run my cc251_mycontrol.sas without error. It will replace the
    the SAS datasets, logs and printed output in sasdata/control, created when I ran cc251_mycontrol.sas

    You will find

    log in                  d:/cps/output/logs/control.log
    print output in         d:/cps/output/logs/control.txt
    SAS code                d:/cps/output/logs/cc251_mycontrol.sas

    * __       _     _
     / _| ___ | | __| | ___ _ __ ___
    | |_ / _ \| |/ _` |/ _ \ '__/ __|
    |  _| (_) | | (_| |  __/ |  \__ \
    |_|  \___/|_|\__,_|\___|_|  |___/

    ;

    This directory stucture has all the inputs you need to run the program.
    These inputs are documeted within the program and odf files.


       ROOT     PATH

      d:/cps
      d:/cps    sascatalog

      d:/cps    data_other
      d:/cps       data_other/plandtal.dat

      d:/cps    pdf
      d:/cps       pdf/2015-instructions-for-analyzing-data.pdf
      d:/cps       pdf/preparing-data-for-analysis.pdf

      d:/cps    programs
      d:/cps       programs/macro-cahps41c.sas
      d:/cps       programs/cc251_control.sas
      d:/cps       programs/cc251_mycontrol.sas   * just run this one
      d:/cps       programs/cc252_format.sas
      d:/cps       programs/cc254_smalltest.sas
      d:/cps       programs/cc255_test.sas
      d:/cps       programs/macro-cahps41c.sas
      d:/cps       programs/make_plandtal_dat.sas

      d:/cps    output
      d:/cps       output/control.txt           * printed output
      d:/cps       output/logs
      d:/cps         output/logs/control.log    * full log

      d:/cps    sasdata
      d:/cps       sasdata/cc252_format.sas
      d:/cps       sasdata/cc254_smalltest.sas
      d:/cps       sasdata/cc257_test.sas7bdat
      d:/cps       sasdata/cc259_test_windows.sas7bdat

      d:/cps-      sasdata/control
      d:/cps-         sasdata/control/c_need.sas7bdat
      d:/cps-         sasdata/control/c_q31.sas7bdat
      d:/cps-         sasdata/control/c_q38.sas7bdat
      d:/cps-         sasdata/control/c_quick.sas7bdat
      d:/cps-         sasdata/control/dpneed.sas7bdat
      d:/cps-         sasdata/control/dpq31.sas7bdat
      d:/cps-         sasdata/control/dpq38.sas7bdat
      d:/cps-         sasdata/control/dpquick.sas7bdat
      d:/cps-         sasdata/control/lrneed.sas7bdat
      d:/cps-         sasdata/control/lrq31.sas7bdat
      d:/cps-         sasdata/control/lrq38.sas7bdat
      d:/cps-         sasdata/control/lrquick.sas7bdat
      d:/cps          sasdata/control/n_need.sas7bdat
      d:/cps          sasdata/control/n_q31.sas7bdat
      d:/cps          sasdata/control/n_q38.sas7bdat
      d:/cps          sasdata/control/n_quick.sas7bdat
      d:/cps          sasdata/control/oaneed.sas7bdat
      d:/cps          sasdata/control/oaq31.sas7bdat
      d:/cps          sasdata/control/oaq38.sas7bdat
      d:/cps          sasdata/control/oaquick.sas7bdat
      d:/cps          sasdata/control/p_need.sas7bdat
      d:/cps          sasdata/control/p_q31.sas7bdat
      d:/cps          sasdata/control/p_q38.sas7bdat
      d:/cps          sasdata/control/p_quick.sas7bdat
      d:/cps          sasdata/control/r2need.sas7bdat
      d:/cps          sasdata/control/r2q31.sas7bdat
      d:/cps          sasdata/control/r2q38.sas7bdat
      d:/cps          sasdata/control/r2quick.sas7bdat
      d:/cps          sasdata/control/saneed.sas7bdat

    *                          _                    _               _
     ___  __ _ _ __ ___  _ __ | | ___    ___  _   _| |_ _ __  _   _| |_
    / __|/ _` | '_ ` _ \| '_ \| |/ _ \  / _ \| | | | __| '_ \| | | | __|
    \__ \ (_| | | | | | | |_) | |  __/ | (_) | |_| | |_| |_) | |_| | |_
    |___/\__,_|_| |_| |_| .__/|_|\___|  \___/ \__,_|\__| .__/ \__,_|\__|
                        |_|                            |_|
    ;



    Rating Scale (0 - 10): Rating Health Plan
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS

    *---------------------------------------------*
      CAHPS SAS Analysis Program Version 4.1
      Report run on 3 March 2020 at 17:06:40
    *---------------------------------------------*


       **********   WARNING NOTE   **********
          PLANS WITH FEWER THAN 100 CASES
    --------------------------------------------

      Plan ID 2 - HMO_B_RURAL  - 95 Cases

      Plan ID 4 - HMO_C_RURAL  - 69 Cases


    --------------------------------------------


     The Variable Item             = q38
     The Variable Type             = 2
     The 2 Adjuster Variables      = ghr age

     Global Case Mix Model
     Global Centering of Means


     The RECODE   parameter        = 0
     The MIN_RESP parameter        = 0
     The MAX_RESP parameter        = 10
     The NAME     parameter        = Rating Health Plan
     The ADJ_BARS parameter        = 1
     The BAR_STAT parameter        = 0
     The IMPUTE   parameter        = 1
     The EVEN_WGT parameter        = 1
     The KP_RESID parameter        = 0
     The ADULTKID parameter        = 3
     The VISITS   parameter        = 1
     The PVALUE   parameter        = 0.05
     The CHANGE   parameter        = 0
     The MEANDIFF parameter        = 0
     The WGTDATA  parameter        = 1
     The WGTRESP  parameter        =
     The WGTMEAN  parameter        =
     The WGTPLAN  parameter        = 0
     The ID_RESP  parameter        =
     The SUBSET   parameter        = 1
     The SPLITFLG parameter        = 0
     The data set used             = adult
     The OUTREGRE parameter        = 0
     The output data set suffix    = q38


    Rating Scale (0 - 10): Rating Health Plan
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    PERCENT ITEMS MISSING BY HEALTH PLAN

                                      Global      General
                     Total # of       Rating       Health       Age of
    Health Plan     Respondents      of Plan       Rating        Adult

    HMO_A_URBAN             345      30.43%        0.58%        1.16%
    HMO_B_RURAL             134      29.10%        0.75%        1.49%
    HMO_B_URBAN             530      24.15%        0.94%        1.70%
    HMO_C_RURAL              90      23.33%        2.22%        0.00%
    HMO_C_URBAN             874      29.18%        0.92%        0.69%



    Report run on 3 March 2020 at 17:06:40
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.p_q38


    Rating Scale (0 - 10): Rating Health Plan
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    PERCENT RESPONSE TYPE - NO IMPUTATIONS

                                    Number of
                    Total # of    Respondents    % Rating    % Rating    % Rating    Adjusted
    Health Plan    Respondents       Analyzed       0 - 6       7 - 8       9 -10       Bar 1

    HMO_A_URBAN            345            240     17.08%      37.50%      45.42%      17.66%
    HMO_B_RURAL            134             95     21.05%      38.95%      40.00%      20.81%
    HMO_B_URBAN            530            402     15.92%      34.08%      50.00%      16.02%
    HMO_C_RURAL             90             69     15.94%      33.33%      50.72%      15.38%
    HMO_C_URBAN            874            619     15.19%      38.93%      45.88%      15.33%

                                             Weighted      Weighted      Weighted
                   Adjusted     Adjusted    Unadjusted    Unadjusted    Unadjusted
    Health Plan       Bar 2        Bar 3      Bar 1         Bar 2         Bar 3

    HMO_A_URBAN     37.99%       44.35%       17.08%        37.50%        45.42%
    HMO_B_RURAL     39.35%       39.84%       21.05%        38.95%        40.00%
    HMO_B_URBAN     33.90%       50.09%       15.92%        34.08%        50.00%
    HMO_C_RURAL     32.57%       52.05%       15.94%        33.33%        50.72%
    HMO_C_URBAN     38.98%       45.69%       15.19%        38.93%        45.88%



    Report run on 3 March 2020 at 17:06:40
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.n_q38


    Rating Scale (0 - 10): Rating Health Plan
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    REGRESSION COEFFICIENTS FOR ADJUSTER VARIABLES

    Variable             Subset
      Name      SPLIT     Name              Q38

      GHR         0      GLOBAL         -0.4171
      AGE         0      GLOBAL          0.3131



    Report run on 3 March 2020 at 17:06:40
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.c_q38


    Rating Scale (0 - 10): Rating Health Plan
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    R-SQUARED VALUES for DEPENDENT VARIABLES

             Subset    Dependent                        Adjusted
    SPLIT     Name     variable        R-squared       r-squared

      0      GLOBAL       Q38             0.0765          0.0752

    Report run on 3 March 2020 at 17:06:40
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.r2q38


    Rating Scale (0 - 10): Rating Health Plan
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    P-Value For Contrast = 0.05 - Change > 0 - Meandiff > 0
    Overall Statistics from t-test
    Ho:  Plan Means All Equal

    Subset     Overall
     Name         Mean         DFR           DFE    F-Statistic     P-Value

    GLOBAL      7.9767           4         1,418       1.4239        0.2237




    Report run on 3 March 2020 at 17:06:40
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.oaq38


    Rating Scale (0 - 10): Rating Health Plan
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    P-Value For Contrast = 0.05 - Change > 0 - Meandiff > 0
    ALL PLANS

                                                                                   Plan Diff.
                                   # of       Unweighted    Weighted    Adjusted      From
                  Total # of    Respondents   Unadjusted   Unadjusted     Plan      Overall
     Plan Name    Respondents    Analyzed     Plan Mean    Plan Mean      Mean        Mean

    HMO_A_URBAN          345           240       7.9708       7.9708      7.9284     -0.0483
    HMO_B_RURAL          134            95       7.7053       7.7053      7.7148     -0.2619
    HMO_B_URBAN          530           402       8.1493       8.1493      8.1460      0.1693
    HMO_C_RURAL           90            69       7.9855       7.9855      8.0311      0.0543
    HMO_C_URBAN          874           619       8.0727       8.0727      8.0633      0.0866

                                +/- 95%
                  Std Error      Conf.      Variance
                      of        Limit of     of the
     Plan Name    Difference     Diff.        Mean      Rating     Plan Weight

    HMO_A_URBAN      0.1081       0.2119      0.0123      **              1.00
    HMO_B_RURAL      0.1602       0.3140      0.0356      **              1.00
    HMO_B_URBAN      0.0922       0.1807      0.0070      **              1.00
    HMO_C_RURAL      0.1817       0.3560      0.0478      **              1.00
    HMO_C_URBAN      0.0832       0.1631      0.0044      **              1.00




    Report run on 3 March 2020 at 17:06:40
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.saq38


    Rating Scale (0 - 10): Rating Quality of Care
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS

    *---------------------------------------------*
      CAHPS SAS Analysis Program Version 4.1
      Report run on 3 March 2020 at 17:07:02
    *---------------------------------------------*


       **********   WARNING NOTE   **********
          PLANS WITH FEWER THAN 100 CASES
    --------------------------------------------

      Plan ID 4 - HMO_C_RURAL  - 74 Cases


    --------------------------------------------


     The Variable Item             = q31
     The Variable Type             = 2
     The 2 Adjuster Variables      = ghr age

     Global Case Mix Model
     Global Centering of Means


     The RECODE   parameter        = 0
     The MIN_RESP parameter        = 0
     The MAX_RESP parameter        = 10
     The NAME     parameter        = Rating Quality of Care
     The ADJ_BARS parameter        = 0
     The BAR_STAT parameter        = 0
     The IMPUTE   parameter        = 1
     The EVEN_WGT parameter        = 1
     The KP_RESID parameter        = 0
     The ADULTKID parameter        = 3
     The VISITS   parameter        = 1
     The PVALUE   parameter        = 0.05
     The CHANGE   parameter        = 0
     The MEANDIFF parameter        = 0
     The WGTDATA  parameter        = 1
     The WGTRESP  parameter        =
     The WGTMEAN  parameter        =
     The WGTPLAN  parameter        = 0
     The ID_RESP  parameter        =
     The SUBSET   parameter        = 1
     The SPLITFLG parameter        = 0
     The data set used             = adult
     The OUTREGRE parameter        = 0
     The output data set suffix    = q31


    Rating Scale (0 - 10): Rating Quality of Care
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    PERCENT ITEMS MISSING BY HEALTH PLAN

                                      Global      General
                     Total # of       Rating       Health       Age of
    Health Plan     Respondents      of Care       Rating        Adult

    HMO_A_URBAN             345      23.19%        0.58%        1.16%
    HMO_B_RURAL             134      23.88%        0.75%        1.49%
    HMO_B_URBAN             530      21.13%        0.94%        1.70%
    HMO_C_RURAL              90      17.78%        2.22%        0.00%
    HMO_C_URBAN             874      20.37%        0.92%        0.69%




    Report run on 3 March 2020 at 17:07:02
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.p_q31


    Rating Scale (0 - 10): Rating Quality of Care
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    PERCENT RESPONSE TYPE - NO IMPUTATIONS

                                      Number of
                     Total # of     Respondents     % Rating     % Rating     % Rating
    Health Plan     Respondents        Analyzed        0 - 6        7 - 8        9 -10

    HMO_A_URBAN             345             265      13.21%       41.13%       45.66%
    HMO_B_RURAL             134             102      14.71%       44.12%       41.18%
    HMO_B_URBAN             530             418      14.83%       40.19%       44.98%
    HMO_C_RURAL              90              74      20.27%       28.38%       51.35%
    HMO_C_URBAN             874             696      15.23%       37.21%       47.56%





    Report run on 3 March 2020 at 17:07:02
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.n_q31


    Rating Scale (0 - 10): Rating Quality of Care
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    REGRESSION COEFFICIENTS FOR ADJUSTER VARIABLES

    Variable             Subset
      Name      SPLIT     Name              Q31

      GHR         0      GLOBAL         -0.2813
      AGE         0      GLOBAL          0.2693

    Report run on 3 March 2020 at 17:07:02
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.c_q31


    Rating Scale (0 - 10): Rating Quality of Care
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    R-SQUARED VALUES for DEPENDENT VARIABLES

             Subset    Dependent                        Adjusted
    SPLIT     Name     variable        R-squared       r-squared

      0      GLOBAL       Q31             0.0467          0.0455


    Report run on 3 March 2020 at 17:07:02
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.r2q31


    Rating Scale (0 - 10): Rating Quality of Care
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    P-Value For Contrast = 0.05 - Change > 0 - Meandiff > 0
    Overall Statistics from t-test
    Ho:  Plan Means All Equal

    Subset     Overall
     Name         Mean         DFR           DFE    F-Statistic     P-Value

    GLOBAL      8.1078           4         1,548       0.2099        0.9330

    Report run on 3 March 2020 at 17:07:02
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.oaq31


    Rating Scale (0 - 10): Rating Quality of Care
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    P-Value For Contrast = 0.05 - Change > 0 - Meandiff > 0
    ALL PLANS

                                                                                   Plan Diff.
                                   # of       Unweighted    Weighted    Adjusted      From
                  Total # of    Respondents   Unadjusted   Unadjusted     Plan      Overall
     Plan Name    Respondents    Analyzed     Plan Mean    Plan Mean      Mean        Mean

    HMO_A_URBAN          345           265       8.1774       8.1774      8.1778      0.0700
    HMO_B_RURAL          134           102       8.0294       8.0294      8.0268     -0.0809
    HMO_B_URBAN          530           418       8.1244       8.1244      8.1199      0.0121
    HMO_C_RURAL           90            74       8.0541       8.0541      8.0646     -0.0432
    HMO_C_URBAN          874           696       8.1537       8.1537      8.1498      0.0420

                                +/- 95%
                  Std Error      Conf.      Variance
                      of        Limit of     of the
     Plan Name    Difference     Diff.        Mean      Rating     Plan Weight

    HMO_A_URBAN      0.1006       0.1971      0.0107      **              1.00
    HMO_B_RURAL      0.1358       0.2661      0.0245      **              1.00
    HMO_B_URBAN      0.0886       0.1737      0.0069      **              1.00
    HMO_C_RURAL      0.1781       0.3492      0.0467      **              1.00
    HMO_C_URBAN      0.0790       0.1549      0.0042      **              1.00


    Report run on 3 March 2020 at 17:07:02
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.saq31


    How Often (1 - 4): Getting Care Quickly
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS

    *---------------------------------------------*
      CAHPS SAS Analysis Program Version 4.1
      Report run on 3 March 2020 at 17:07:10
    *---------------------------------------------*


       **********   WARNING NOTE   **********
          PLANS WITH FEWER THAN 100 CASES
    --------------------------------------------

      Plan ID 4 - HMO_C_RURAL  - 74 Cases


    --------------------------------------------


     The 4 Variable Items          = q15 q17 q19 q24
     The Variable Type             = 3
     The 2 Adjuster Variables      = ghr age

     Global Case Mix Model
     Global Centering of Means


     The RECODE   parameter        = 0
     The MIN_RESP parameter        = 1
     The MAX_RESP parameter        = 4
     The NAME     parameter        = Getting Care Quickly
     The ADJ_BARS parameter        = 0
     The BAR_STAT parameter        = 0
     The IMPUTE   parameter        = 1
     The EVEN_WGT parameter        = 1
     The KP_RESID parameter        = 0
     The ADULTKID parameter        = 3
     The VISITS   parameter        = 1
     The PVALUE   parameter        = 0.05
     The CHANGE   parameter        = 0
     The MEANDIFF parameter        = 0
     The WGTDATA  parameter        = 1
     The WGTRESP  parameter        =
     The WGTMEAN  parameter        =
     The WGTPLAN  parameter        = 0
     The ID_RESP  parameter        =
     The SUBSET   parameter        = 1
     The SPLITFLG parameter        = 0
     The data set used             = adult
     The OUTREGRE parameter        = 0
     The output data set suffix    = quick


    How Often (1 - 4): Getting Care Quickly
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    PERCENT ITEMS MISSING BY HEALTH PLAN

                                                                Wait in
                               Get the   Get and    Get Care        the   General
                  Total # of  help you Appointment as soon as   Doctors    Health    Age of
    Health Plan  Respondents    Needed when Wanted   Wanted      Office    Rating     Adult

    HMO_A_URBAN          345   55.94%     46.38%     47.25%     40.00%     0.58%     1.16%
    HMO_B_RURAL          134   63.43%     46.27%     45.52%     39.55%     0.75%     1.49%
    HMO_B_URBAN          530   57.74%     41.89%     46.98%     35.85%     0.94%     1.70%
    HMO_C_RURAL           90   66.67%     43.33%     54.44%     31.11%     2.22%     0.00%
    HMO_C_URBAN          874   55.84%     49.77%     48.63%     37.64%     0.92%     0.69%



    Report run on 3 March 2020 at 17:07:10
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.p_quick


    How Often (1 - 4): Getting Care Quickly
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    PERCENT RESPONSE TYPE - NO IMPUTATIONS

                                                       %
                                      Number of    Sometimes
                     Total # of     Respondents    or Never     % Usually     % Always
    Health Plan     Respondents        Analyzed       1-2           3                4

    HMO_A_URBAN             345             270      19.13%       20.39%       60.48%
    HMO_B_RURAL             134             107      19.44%       23.32%       57.23%
    HMO_B_URBAN             530             436      17.78%       38.31%       43.91%
    HMO_C_RURAL              90              74      21.32%       20.99%       57.69%
    HMO_C_URBAN             874             688      14.92%       15.69%       69.39%



    Report run on 3 March 2020 at 17:07:10
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.n_quick


    How Often (1 - 4): Getting Care Quickly
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    REGRESSION COEFFICIENTS FOR ADJUSTER VARIABLES

    Variable           Subset
      Name     SPLIT    Name             Q15            Q17            Q19            Q24

      GHR        0     GLOBAL        -0.1665        -0.1099        -0.1347        -0.0473
      AGE        0     GLOBAL         0.1608         0.1099         0.0583         0.0698




    Report run on 3 March 2020 at 17:07:10
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.c_quick


    How Often (1 - 4): Getting Care Quickly
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    R-SQUARED VALUES for DEPENDENT VARIABLES

             Subset    Dependent                        Adjusted
    SPLIT     Name     variable        R-squared       r-squared

      0      GLOBAL       Q15             0.0456          0.0433
      0      GLOBAL       Q17             0.0339          0.0321
      0      GLOBAL       Q19             0.0282          0.0263
      0      GLOBAL       Q24             0.0224          0.0208




    Report run on 3 March 2020 at 17:07:10
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.r2quick


    How Often (1 - 4): Getting Care Quickly
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    P-Value For Contrast = 0.05 - Change > 0 - Meandiff > 0
    Overall Statistics from t-test
    Ho:  Plan Means All Equal

    Subset     Overall
     Name         Mean         DFR           DFE    F-Statistic     P-Value

    GLOBAL      3.3389           4         1,568      16.7924        0.0001



    Report run on 3 March 2020 at 17:07:10
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.oaquick


    How Often (1 - 4): Getting Care Quickly
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    P-Value For Contrast = 0.05 - Change > 0 - Meandiff > 0
    ALL PLANS

                                                                                   Plan Diff.
                                   # of       Unweighted    Weighted    Adjusted      From
                  Total # of    Respondents   Unadjusted   Unadjusted     Plan      Overall
     Plan Name    Respondents    Analyzed     Plan Mean    Plan Mean      Mean        Mean

    HMO_A_URBAN          345           270       3.3323       3.3323      3.3309     -0.0081
    HMO_B_RURAL          134           107       3.3457       3.3457      3.3414      0.0024
    HMO_B_URBAN          530           436       3.2109       3.2109      3.2101     -0.1289
    HMO_C_RURAL           90            74       3.3051       3.3051      3.3091     -0.0299
    HMO_C_URBAN          874           688       3.5006       3.5006      3.5033      0.1644

                                +/- 95%
                  Std Error      Conf.      Variance
                      of        Limit of     of the
     Plan Name    Difference     Diff.        Mean      Rating     Plan Weight

    HMO_A_URBAN      0.0409       0.0801      0.0018     **               4.00
    HMO_B_RURAL      0.0523       0.1024      0.0036     **               4.00
    HMO_B_URBAN      0.0333       0.0652      0.0009     *                4.00
    HMO_C_RURAL      0.0704       0.1379      0.0073     **               4.00
    HMO_C_URBAN      0.0290       0.0568      0.0005     ***              4.00



    Report run on 3 March 2020 at 17:07:10
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.saquick


    Trichotomous Variable (1 - 3): Getting Care Needed
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS

    *---------------------------------------------*
      CAHPS SAS Analysis Program Version 4.1
      Report run on 3 March 2020 at 17:07:21
    *---------------------------------------------*


       **********   WARNING NOTE   **********
          PLANS WITH FEWER THAN 100 CASES
    --------------------------------------------

      Plan ID 4 - HMO_C_RURAL  - 89 Cases


    --------------------------------------------


     The 4 Variable Items          = q06 q10 q22 q23
     The Variable Type             = 4
     The 2 Adjuster Variables      = ghr age

     Global Case Mix Model
     Global Centering of Means


     The RECODE   parameter        = 0
     The MIN_RESP parameter        = 1
     The MAX_RESP parameter        = 3
     The NAME     parameter        = Getting Care Needed
     The ADJ_BARS parameter        = 0
     The BAR_STAT parameter        = 0
     The IMPUTE   parameter        = 1
     The EVEN_WGT parameter        = 1
     The KP_RESID parameter        = 0
     The ADULTKID parameter        = 3
     The VISITS   parameter        = 1
     The PVALUE   parameter        = 0.05
     The CHANGE   parameter        = 0
     The MEANDIFF parameter        = 0
     The WGTDATA  parameter        = 1
     The WGTRESP  parameter        =
     The WGTMEAN  parameter        =
     The WGTPLAN  parameter        = 0
     The ID_RESP  parameter        =
     The SUBSET   parameter        = 1
     The SPLITFLG parameter        = 0
     The data set used             = adult
     The OUTREGRE parameter        = 0
     The output data set suffix    = need


    Trichotomous Variable (1 - 3): Getting Care Needed
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    PERCENT ITEMS MISSING BY HEALTH PLAN

                               Problem Problem to  Problem in   Delay in   General
                  Total # of  to get a   get a    Getting Care   getting    Health    Age of
    Health Plan  Respondents    Doctor  Referral     Needed     Approval    Rating     Adult

    HMO_A_URBAN          345   61.16%    30.43%      31.01%       2.90%     0.58%     1.16%
    HMO_B_RURAL          134   65.67%    29.10%      29.10%       5.22%     0.75%     1.49%
    HMO_B_URBAN          530   62.83%    24.34%      24.53%       2.26%     0.94%     1.70%
    HMO_C_RURAL           90   71.11%    23.33%      23.33%       2.22%     2.22%     0.00%
    HMO_C_URBAN          874   60.64%    28.72%      28.83%       2.52%     0.92%     0.69%

    Report run on 3 March 2020 at 17:07:21
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.p_need


    Trichotomous Variable (1 - 3): Getting Care Needed
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    PERCENT RESPONSE TYPE - NO IMPUTATIONS

                                      Number of
                     Total # of     Respondents      % Big       % Small      % Not a
    Health Plan     Respondents        Analyzed    Problem 1    Problem 2    Problem 3

    HMO_A_URBAN             345             340      17.79%       20.06%       62.14%
    HMO_B_RURAL             134             130      18.84%       21.65%       59.51%
    HMO_B_URBAN             530             523      16.79%       18.35%       64.86%
    HMO_C_RURAL              90              89      17.87%       22.37%       59.76%
    HMO_C_URBAN             874             864      18.36%       18.23%       63.41%




    Report run on 3 March 2020 at 17:07:21
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.n_need


    Trichotomous Variable (1 - 3): Getting Care Needed
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    REGRESSION COEFFICIENTS FOR ADJUSTER VARIABLES

    Variable           Subset
      Name     SPLIT    Name             Q06            Q10            Q22            Q23

      GHR        0     GLOBAL        -0.0388        -0.0501        -0.0694        -0.0432
      AGE        0     GLOBAL         0.0717         0.0428         0.0499         0.0825



    Report run on 3 March 2020 at 17:07:21
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.c_need


    Trichotomous Variable (1 - 3): Getting Care Needed
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    R-SQUARED VALUES for DEPENDENT VARIABLES

             Subset    Dependent                        Adjusted
    SPLIT     Name     variable        R-squared       r-squared

      0      GLOBAL       Q06             0.0134          0.0108
      0      GLOBAL       Q10             0.0196          0.0182
      0      GLOBAL       Q22             0.0298          0.0284
      0      GLOBAL       Q23             0.0161          0.0151



    Report run on 3 March 2020 at 17:07:21
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.r2need


    Trichotomous Variable (1 - 3): Getting Care Needed
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    P-Value For Contrast = 0.05 - Change > 0 - Meandiff > 0
    Overall Statistics from t-test
    Ho:  Plan Means All Equal

    Subset     Overall
     Name         Mean         DFR           DFE    F-Statistic     P-Value

    GLOBAL      2.4401           4         1,939       0.8414        0.4988


    Report run on 3 March 2020 at 17:07:21
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.oaneed


    Trichotomous Variable (1 - 3): Getting Care Needed
    Analysis = ADULTS ONLY  -  Visits = COMBINE LOW AND HIGH USERS
    P-Value For Contrast = 0.05 - Change > 0 - Meandiff > 0
    ALL PLANS

                                                                                   Plan Diff.
                                   # of       Unweighted    Weighted    Adjusted      From
                  Total # of    Respondents   Unadjusted   Unadjusted     Plan      Overall
     Plan Name    Respondents    Analyzed     Plan Mean    Plan Mean      Mean        Mean

    HMO_A_URBAN          345           340       2.4435       2.4435      2.4416      0.0015
    HMO_B_RURAL          134           130       2.4068       2.4068      2.4069     -0.0331
    HMO_B_URBAN          530           523       2.4807       2.4807      2.4812      0.0411
    HMO_C_RURAL           90            89       2.4189       2.4189      2.4182     -0.0218
    HMO_C_URBAN          874           864       2.4504       2.4504      2.4524      0.0123

                                +/- 95%
                  Std Error      Conf.      Variance
                      of        Limit of     of the
     Plan Name    Difference     Diff.        Mean      Rating     Plan Weight

    HMO_A_URBAN      0.0255       0.0499      0.0007      **              4.00
    HMO_B_RURAL      0.0391       0.0766      0.0021      **              4.00
    HMO_B_URBAN      0.0230       0.0451      0.0004      **              4.00
    HMO_C_RURAL      0.0452       0.0886      0.0030      **              4.00
    HMO_C_URBAN      0.0209       0.0409      0.0003      **              4.00



    Report run on 3 March 2020 at 17:07:21
    CAHPS SAS Analysis Program Version 4.1
    Data Set out.saneed


