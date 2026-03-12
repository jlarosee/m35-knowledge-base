# TOP OF MIND

Hydrator is fucking up contacts
https://www.notion.so/emporia/Hydration-service-is-creating-incomplete-contact-records-31ac3dd5414780db8191e60def8d1d5c

-----------

# mar 13
- all hands
  - What's shipped
    - Video question type in surveys - A brand new question type that allows respondents to answer questions via video, plus playback and transcription in managed respondents table. HUGE shoutout to @huan and @lijin.
    - RFQ screener download - Suppliers now have access to project screener files in Levada to help inform them of the audience.
    - RFQ notifications refresh - centralization of RFQ notifications into single email threads, which will help both admin and suppliers communicate around projects.
  - What's shipping next week
    - As an Emporia Supplier, I want the option to not have to submit feasibility on RFQs
    - Qual-at-scale projects to function correctly with proper prescreening, payout timing, and reporting metrics
    - Polis User, I want the mobile navbar to collapse into a hamburger menu
    - Charge job updates - accurately calculating our win vs delivery rate on projects
  - Demos
    - RFQ Screener download
    - Video Question type + playback and transcription
      - https://www.loom.com/share/1ba260bdc6c242da80b8e95a9526e770
    - RFQ notifications refresh
 

# mar 12
- RFQ "maven" ticket - "option to not have to submit feasibility on RFQs"
  - cleaned up and PR'd
  - will @chris for CR
- get update-campaign dedupe merged
  - https://github.com/Emporia-Research/EmporiaSharedBackend/pull/1024#pullrequestreview-3933410295
- 

# mar 11
- DE
  - bump gmass6 ✅
  - check risky drops metric ✅
- RFQ CR addressed ✅ WILL MERGE 
- on-call catchup ✅
  - PR'd 
    - update-campaign bug
    - DE router metric build bug
- supplier tagging sync later ✅
- RF workflow docs

- get shipped
  - EMP-3599: Feat/update: allow partner verification methods to be modified 


# mar 10
- RF sample collection coverage STARTS NEXT WEEK
  - Add "Test Ticket" to ticket templates ✅
- core release help ✅
- dug into some on-call
- PR'd Feat/update: allow partner verification methods to be modified in the segment drawer UI ✅
- PR'd feature flagging the agent/synth ui in core - EMP-3593 ✅


# mar 9
- Mission checkin - stack review
- bit of oncall
- demo'd RFQ email threading for chris'
- CR for lijin


# mar 6
- OA ✅
- rfq notifications ✅
- rfq auto-accept ✅
- intro call with another vendor, Mission at 12:30 ✅
- get an archicture doc to caylent ✅
  - BETTER labels ❌
- agent harness work ✅


# mar 5
- call w/ caylent - vendor who might help w/ our migration
  - intro with another vendor today - Mission
- rfq notifications
    * continue working out the threading issue ✅
    * Figured out much of threading ✅
- rainforest sync later ✅
- DE failure investigation
  - sync'd w/ brandon about malformed contacts ✅
  - discovery w/ claude to ID possible bugs in hydration_service
    - cut a ticket 🎟️


# mar 4
- mark RF test flow ✅
    * created a new "how to" doc ✅
- finish rfq notifications ❌
    * worked on threading
- cr for brando's rehydration ✅
- worked on s3 cors issues on video response branch
    * pr'd an update to override.ts for main ✅
    * fixed it! ✅
- DE router bump gmass6 send +500 ✅
- looked into DE router failures - created a new alarm ✅
    * we have contacts without emails which is failing on domian extraction
- started on rfq auto-accept ✅
    * got it working - need to do final tests; new branch


# mar 3
- finish rfq notifications
    * template review w/ rach and chris
- started cr for brando's rehydration
- interview loop
- RF proposal to chris and jase for review
- will be out starting at 2pm PST

# mar 2
- get rfq notifications PR'd
    * sync'd w/ chris on email templates and copy
    * updated
- supplier bids auto-accepted
- huan
    * finished cr
- tried to get tembo to work
- sync w/ ando on Rainforest workflow change proposal
    * https://www.notion.so/emporia/RF-Eng-Test-Workflow-Proposal-317c3dd5414780e8b7feef47f6e674c8

   

# feb 27
- manager training roundtable 
- cr huan
    * spent time trying to get the env working to do a full test loop
    * FINISH WEB CR
- ✅ levada screener shipped
- rfq notifications started
    * just about done but need to sync w/ chris on some copy and email desing updates

- bug ticket automatin
- dd ticket generation 
- notion ticket picks
- notion ticket cutter

# feb 26

- ✅ supplier portal release out
- ✅ core release out - @jordo!
- ✅ jordo CR for reco
- loom demos for tomorrow
    * ✅ lijin loader 
    * qual non-autoblend JOSH
    * screener download in RFQ JOSH ❌ - not ready
    * PO copy button in core RFQ / Segment drawers JOSH
    * hackathon playback service JOSH
- ✅ huan CR for transcription
- DE
    * 🚨 risky inbox drop metric broken
    * bump cold engage +300
- start RFQ notifications ticket
- 🚨 risky increase?
    * 🐞 we're not properly throttling risky atm

# feb 25

- ✅ mailsoar sync
    * synced w/ jase on strategy for getting the segment data through to external email event api handler
- ✅ landed PRs for supplier updates
- ✅ had call with AWS about Signature Expire 
    * they really need a HAR file to debug on their end
    * https://repost.aws/knowledge-center/support-case-browser-har-file
- ✅ pinged RF about a failed levada test and extending coverage to screener download
- ✅ started on huan's transcription PR - will focus on that today


# feb 24
- worked on email validation tier and segment in the event metadata (EMP-3403)
    * https://github.com/Emporia-Research/EmporiaEngineWeb/pull/1976
    * scheduled sync w/ jase to review the segment AC
- updated the risky inbox metrics
- posted updates to DE channel on new cold open performance
- synced w/ andrew on update-campaign errors - pr'd a fix to dedupe batch write emails during update_campaign
- worked w/ huan a bit to update claude configs repo - got it merged
- PR for EMP-3534 - Render link to open screener / files in RFQ drawer
- PR for EMP-3537 - Prevent auto RFQ flow on non-quant projects 
- started EMP-3535 show-po-for-rfqs-and-segments-in-core-segments-ui

# feb 23
- ✅ OAs
    * https://coderbyte.com/report/userrggzybl4b:technical-assessment-md42qnu01l
    * https://coderbyte.com/report/userog1lc5lye:technical-assessment-md42qnu01l
- ✅ cold open released
- ✅ risky inbox ratios released
- Updated DE channel
- ✅ VERISOUL retry
    * ticket, handed off to on-call
- ✅ get CR for levada redirects ticket
    * bugfix/jl/EMP-3199/fix-auth-context
    * @ando
- get CR for email validation in reporting event body
    * jl/update/EMP-3403/include-email-validation-tier-in-reporting-metadata 
- ✅ EmporiaAI PR
    * https://github.com/Emporia-Research/EmporiaAI/pull/1
- ✅ AWS support case follow-up
    * scheduled for 25th - invited @jordo to join (on-call)

# feb 13
- mailsoar
    * emails for pierre to verify the waterfall strategy
        + we'll run the batch to waterfall and get that list
- ✅ warmups job updated / deployed - no experimental templates 
- interview
- ✅ ship verisoul update to polis
    * release
    * 🚨 New alarm for verisoul failures
- merged core: currentVerificationMethods now uses partner if available
- ✅ light investigation of Layer14 (solicitation generation) - still invoked
    * cut a ticket to flag it off
- risky inbox merged
    * ✅ merged!
    * deployed ❌
- finish the levada redirects ticket - started yesterday
- email validation tier event metadata into the DD and mailsoar payloads


# feb 12
- follow up w/ AWS on the signature expiration ticket ✅ 2026-02-12
- grooming ✅ 2026-02-12
- started on the login redirects in Levada
- synced w/ ando on polis errors ✅ 2026-02-12
    * incentives
    * verisoul session ids not coming back from verisoul ✅ 2026-02-12
    * looked into some polis logs per Jase ✅ 2026-02-12
- addressed cr comments for "risky inbox" provider PR - i answered a couple comments
    * ready to ship
- cr for ando
- Bit of prep for next week
    * claude deck

# feb 11
- raise a ticket w/ AWS on the session expire 🚨
- sync w/ ando on polis error logs audit
- interview loops
- DE tickets 
    * finish the "cold open" ticket
    * get these shipped 



# feb 10
- went back to the Risky SMTP proportional send - fixed some bugs and raised PR
- sync'd w/ jase and andrew on some on-site items




# feb 9
- on-call handoff @ando and a couple tasks that i need to finish ✅ 
- interview ✅
    * went pretty well - maybe a jr candidate
- release admin
    * adding grace
- ZB seed updated ❌
- requested changes from RF on the VPN tests so that they re-use a static project  ✅
    * getting rid of all the setup boilerplate

# feb 6
- sync'd w/ brandon on api client errors - "destructuring payload" and the respondentData:
    * PR raised
- sync'd w/ jase on errors i'd been working on throughout the week
    - verisoul failures
        * PR raised 
    - ms safe links - handled w/ recatpch
    - surveyWrapper fetching twice - STILL trying to repro
    - /collection/sample/validate, /survey, etc - why is it taking so long? not affecting that many real users - lower priority
    - signature expiration - this one is a doozy
- oncall backlog


- Mailsoar TODOs
    * Postmastery MJ payload adjustment
    * investigate some "noise" they're reporting on their end
- VI links - why not working in admin?
- CR for ando
    * RFQ notes
- on-call ticket backlog ✅
- Rainforest
    * look at why those few tests are still failing
    * check in on requested updates
    * another request to RF to extend sample collection coverage 
- OA - https://coderbyte.com/report/userxenqg8f0s:technical-assessment-md42qnu01l
- error log tickets ✅ 
    * "TypeError: Cannot destructure property 'survey' of 't.payload' as it is undefined.”
    * Fetch error GET (route/session)
        + https://us5.datadoghq.com/logs?query=%22%2Fmain%2Fcollection%2Froute%2Fsession%22%20status%3Aerror&agg_m=count&agg_m_source=base&agg_t=count&clustering_pattern_field_path=message&cols=host%2Cservice&context_event=AZwlE8eLAAC4TMQWL4uvDAAB&fromUser=true&messageDisplay=inline&refresh_mode=sliding&storage=hot&stream_sort=time%2Cdesc&viz=&from_ts=1767559558243&to_ts=1770151558243&live=true
- RF coverage ext
    * survey links


# feb 5
- on-call ticket backlog from the week
    * we've had 4 requests this week for direct Virtual incentive redemption links
- Mailsoar - sent the MJ body to pierre for review
    * heard back from him today and will look at making an update based on his response 
- did a deep dive into the update campaign lambda failure with andrew
    * we boiled it down to the sqs message reader timing out  

# feb 4
- core release - rfq
- admin release - sourcing segment id fix
- worked w/ lijin a bit on googlesheet deployment
- on-call tickets to catch up on
    * signature expired (affecting polis users) seems to have cleared up
- continue log investigation across polis
- finish the MS/outlook ticket + investigation
    * does hitting links create PC and then the PC state causes follow on errors? (destructuring survey??)
- OA
    * https://coderbyte.com/report/user5ow0dmauc:technical-assessment-md42qnu01l
    * https://coderbyte.com/report/userejo3hlijw:technical-assessment-md42qnu01l
    * https://coderbyte.com/report/usergmr00ebno:technical-assessment-md42qnu01l

# feb 3
- cut tickets from the log audit
    * cut 3 - review w/ jase
- on-call tickets to review
- chris - cr for DE
    * pending gmass3 increase for unknown status
- RF coverge update request - RFQ
    * loom'd
- RFQ release
    * supplier portal released
    * core - waiting

# feb 2
- on-call handoff w/ jordan and jase
- closeout + planning
- OA - https://coderbyte.com/report/usern6qnyjfx4:technical-assessment-md42qnu01l
- log audit 
- land rfq today
    * talk next steps with chris and dana
    - BUG FIX 🚨
        * https://github.com/Emporia-Research/EmporiaSharedBackend/pull/972
        * https://github.com/Emporia-Research/EmporiaSupplierPortal/pull/160

# jan 30
- out in the AM - thx brando for covering the all hands update
- rfq - addressed cr comments
- sync'd w/ ando on some items for on-site

# jan 29
- Crs
    * brando
    * 
- rfq - working through some ant comments
    * sync w/ chris and dana a bit on where we're at and what's next up 
- sync w/ chris and rach on rfq auto-accept
    * sermo - no team config
        + industry == healthcare/mental health (rach), send to sermo
    * rakuten
        + should be on team whitelists
        + no auto-accept (config addition)
    * LINK to the segment rfq in emails
- NEW TICKET: levada: "see my projects" supplier PMs (NEW TICKET) 
- EXISTING TICKET?: Segment name in the PAUSE status notifications

# jan 28
- goals chat w/ jase
- deployed the gmass campaign updater fix
- rfq - raised a PR


# jan 27
- rfq ui 
    * look into wiring up the HS link
    * auto-accept threshold changes
    * sync w/ chris later to touch base
- looked into the gmass campaign updater
    * PR to bump the max queue msgs down 25%
        + will raise today 

# jan 26
- update the warmup seeds today
- rfq update
- postmastery dashboard check

# jan 23
- mailsoar
    * addressed some action items
        + checked our gmass6 metrics
        + postmastery templates ???
- CR
    * brando's audience critiera locking PR
- made progress on the rfq update

# jan 22
- focused on RFQ update ticket
- sync w/ chris on rfqs and email validation

# jan 21
- focused on RFQ workflow update ticket
- looking into the Rainforest failures in core
    * chatting w/ Maksym on this issue
    * VPN checks on 3p even though it's not set ??
- sync'd w/ dana on some RFQ ui changes
    * did CR for those updates - look GOOD
- sync'd w/ lijuin on sample collection testing
- did a coding assessment

- tabled - "cold open" ticket - raise PR

# jan 20
- synced w/ mark on the admin team + parnter ui chagnes and bringing Maven back as auto-blendable
- sync w/ chris on potential issue with email re-validation
    * it looks like we wait too long to re-validate emails which causes use to send to stale addresses and get hard bounced
- started levada RFQ update ticket
    * rounded out some AC
- code assessement
    * https://coderbyte.com/report/user1drt6mm7v:technical-assessment-md42qnu01l

# jan 16
- levada release to fix
    * CSV export
    * segment sample URL rendered after verfication
- synced w/ chris on the 50% email drop ticket
    * think we have a line on a reason and a solution but will want jase's input to move forward with that or call what we have "good"
- started "cold open" email interactions ticket for DE
    * almost done - will raise pr today

# jan 15
- admin release ✅
    * fixed the admin teams ui test in RF ✅
- RFQ sync w/ chris & dana to kickoff that workstream ✅
- raised a PR for the risky SMTP propotional send changes
- CRs
    * brando and lijin
- ROADMAP review https://www.notion.so/emporia/Emporia-2026-Product-Roadmap-All-2e5c3dd5414780709cbef51d27e1c38f ✅


# jan 14
- DE: risky SMTP propotional send ticket
    * progress!
- RF - external survey setup
    * synced w/ chris a little on that
- RFQ updates
    * sync w/ chris on some planning 
    * chat w/ ando on HS integration + conversations

# jan 13
- finally finished admin teams ui CR 
- sync'd with chris on upcoming RFQ workflow changes and "other releavant info" field ideas
- on-call: respondents coming through router marked "public & referral" segment
    * tried to repro - tabling for now
- more work on extending RF survey coverage
    * setup a Typeform account and configured a survey
        + but we need a paid account (300/year)
- DE: started on risky SMTP propotional send ticket
    * which will allow for more granular control over if and how much we send to some ISPs 

# jan 12
- on-call handoff @brando noon ✅
- synced w/ ando on our upcoming RF process changes ✅
- supplier portal release ✅
    * revert otherRelevantInfo (SBE?)
    * segment test ui updates out
- on-call followup 
    * created a project contact record for Danielle on the Strella project ✅
- admin team/partner ui CR done - release
- 🚨 Jase's RF coverage request
    * passed some new tests requests to RF last night ✅
    * need to parse it and create a pipeline

# jan 9
- on-call tasks
    * Mixed Contact Profiles - cary burcham + danielle ID mixup
        + got some input from jase on this one
    * wynter - spent a long time trying to figure this one out
        + somehow the contact was served a direct link to a project with no active segments and they weren't sourced
- RF call to review the annual contract
- 🚨 Jase's RF coverage request
    * need to parse it and create a pipeline

# jan 8
- mailsoar 
    * templates breakdown to pierre 
        + templates subjects to ids ✅ 
- ZB fixed 
    * NM; updated on the 21st ✅ 
- PRs to wrap up:
    * segment test mode 
    * bulk 3p creation ✅
    * admin team UI CRs
- did a core releast late yesterday ✅
- CRs
    * brando's ✅
- on-call
    * tickets
        + respondents coming through router getting marked "public and referral" segment in manage respondents
    * admin alarms this morning
    * polis alarms 
        + verisoul - adblockers (MABYE test w/ adblockers? check jase's log link; probs just seasonal downturn) m35-knowledge-base
M35 Knowledge Base - Personal notes and documentation


Hello!

