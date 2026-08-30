# Changelog

## 1.0.418
- fix(sell): include grid controller capacity in best_result scheduling

## 1.0.417
- fix(sell): fall back to threshold when best_result forecast is empty

## 1.0.416
- feat(telemetry): delete installation, add comments, fix solar/yield values

## 1.0.415
- fix: rename release config template to prevent HA Supervisor collision

## 1.0.414
- fix(grid-controller): default ems_control to empty list (explicit opt-in)

## 1.0.413
- fix(grid-controller): recognize grid_controllers key in config validator and fix take_control default

## 1.0.412
- fix: correct release repo metadata and sync pipeline

## 1.0.411
- ci: add weekly scheduled release (Mondays 08:00 UTC)

## 1.0.410
- fix(integration): preserve user URL on retry and add reconfigure support

## 1.0.409
- fix: include inverters.yaml template in Docker image

## 1.0.408
- fix: meter unit conversion, remove dead EV ems_control, sync spec

## 1.0.407
- feat(release): add auto-sync, dockerignore, update release config to v1.0.406

## 1.0.406
- fix: prevent relay device oscillation and reduce HA write noise

## 1.0.405
- fix: rename package path from ventra-ems-v2 to ventra-ems in workflow and release config

## 1.0.404
- rename: _release/ventra-ems-v2 → _release/ventra-ems

## 1.0.403
- fix: install pytest and pytest-mock inline in test workflow

## 1.0.402
- fix: replace uvicorn[standard] with uvicorn and remove test deps from requirements

## 1.0.401
- fix: install gcc and musl-dev in builder stage for Cython C compilation

## 1.0.400
- fix: remove nthreads from cythonize and pin base images to Python 3.13

## 1.0.399
- fix: correct HA base image tags to :latest in release workflow

## 1.0.398
- feat: add Cython compilation pipeline and multi-arch release workflow

## 1.0.397
- fix: recover EV charger session when Charging state is detected without prior Preparing

## 1.0.396
- fix: correct malformed About nav link across all pages

## 1.0.395
- feat: remove license indicator from header nav

## 1.0.394
- feat: add About page with license status, system info, and device counts

## 1.0.393
- fix(deploy): use ha CLI over SSH instead of broken Supervisor API

## 1.0.392
- feat(deploy): fix pipeline — SSH store refresh, Proxmox service control, version-bump triggers

## 1.0.391
- test: print add-on version on startup

## 1.0.390
- feat: add deploy server for automated HA add-on updates

## 1.0.389
- feat: add local deploy script for automated HA add-on updates

## 1.0.388
- feat(integration): remove orphaned devices when config shrinks

## 1.0.387
- chore: use generic placeholders in ha.env.example

## 1.0.386
- chore: replace bundled inverters.yaml with a generic template

## 1.0.385
- fix: correct Supervisor map key homeassistant → config

## 1.0.384
- fix(run.sh): robust companion install with /config fallback and clean error path

## 1.0.383
- fix(run.sh): detect unmounted /homeassistant before companion install

## 1.0.382
- refactor: three approved cleanup refactors

## 1.0.381
- refactor: readability and cleanup pass across 9 files

## 1.0.380
- security: harden license system against 6 identified vulnerabilities

## 1.0.379
- chore: extract credentials from deploy scripts into env files

## 1.0.378
- chore: rename 'backend server' folder to 'public server'

## 1.0.377
- feat(telemetry): send inverters.yaml config with each installation report

## 1.0.376
- fix(devices): align theme system with all other pages

## 1.0.375
- fix: rewrite fetch URLs for HA ingress compatibility

## 1.0.374
- fix(license): make startup check non-blocking, reduce HTTP timeout

## 1.0.373
- fix(license): retry every 5 min until first successful validation

## 1.0.372
- fix(telemetry): only advance last_report on HTTP 200 OK

## 1.0.371
- fix(telemetry): make reporting thread resilient and surface failures as warnings

## 1.0.370
- fix(telemetry): correct solar and grid energy fields in hourly report

## 1.0.369
- fix: move license_manager.configure() call to after object is created

## 1.0.368
- feat: add license status chip to nav bar on all pages

## 1.0.367
- fix: handle PermissionError in LicenseManager when /data is not writable

## 1.0.366
- latest

## 1.0.365
- chore: update callback domains to ventra-ems.com

## 1.0.364
- security: AES-encrypt license cache, spread output guards across all write methods

## 1.0.363
- feat: add license system and telemetry

## 1.0.362
- feat(devices): add ON/OFF condition mode, per-relay activity log, systemd autostart

## 1.0.361
- fix(control): add price source to buy strategy, fix stale window message, remove caps from window headers

## 1.0.360
- refactor(ems): setpoint filter is per-battery only, no global fallback

## 1.0.359
- feat(devices): move battery inverter settings from control to devices page

## 1.0.358
- fix(nav): anchor dropdown to hamburger button position on all pages

## 1.0.357
- fix(control): refresh buy/sell windows after any settings change

## 1.0.356
- feat(control): add buy strategy with best_result mode and split control page

## 1.0.355
- feat: device condition system enhancements and UI cleanup

## 1.0.354
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.353
- feat: EV power modes, min ON time, and companion integration cleanup

## 1.0.352
- fix(devices): remove top separator line on first relay section

## 1.0.351
- fix(devices): fix status badge visibility and multi-relay header

## 1.0.350
- feat(sensor): automatic unit conversion from HA unit_of_measurement

## 1.0.349
- fix(devices): remove device gate for multi-relay devices

## 1.0.348
- chore(ui): rename condition labels to user-friendly names

## 1.0.347
- feat(conditions): virtual excess budget for solar_excess_above condition

## 1.0.346
- feat(conditions): add solar_excess_above condition with hysteresis

## 1.0.345
- fix(heatpump): make all 4 relays independent — main no longer follows mode relays

## 1.0.344
- feat(devices): add per-relay condition control for heat pump and AC mode relays

## 1.0.343
- fix(ui): use relative font URLs for HA ingress compatibility

## 1.0.342
- fix(devices): use relative API fetch URLs for HA ingress compatibility

## 1.0.341
- fix(devices): show API error on page instead of silently showing empty

## 1.0.340
- fix(api): rename /api/relay_devices to /api/devices

## 1.0.339
- feat(ev-charger): move EV chargers to condition-based control (schema v4)

## 1.0.338
- fix(devices): remove ev_chargers from conditions page; restore ems_control default

## 1.0.337
- fix(devices): fix CSS selector crash on device names with spaces, align nav

## 1.0.336
- feat(devices): replace schedule system with condition-based device control

## 1.0.335
- fix(overview): raise portrait aspect cap to 1.6 to reduce empty space on tall phones

## 1.0.334
- fix(overview): centre Home node vertically by growing viewBoxH to 2×minHomeY

## 1.0.333
- fix(overview): cap diagram height on tall/narrow screens to avoid over-spreading nodes

## 1.0.332
- fix(widget): remove arrow icons from grid connection status labels

## 1.0.331
- fix(widget): Dutch labels for grid connection state (Importeren/Gebalanceerd/Exporteren)

## 1.0.330
- fix(overview): increase bottom padding so device nodes don't overlap fixed footer

## 1.0.329
- fix(widget): remove 'laadt' from battery sub text

## 1.0.328
- fix(widget): label tweaks — NET/BATTERIJ above circles, remove vandaag/ontlaadt

## 1.0.327
- fix(widget): match overview page colours for all nodes and animations

## 1.0.326
- feat(widget): replace emoji icons with SVG icons matching overview page

## 1.0.325
- fix(widget): use real iframe in preview; add explicit width:100% to widget body

## 1.0.324
- fix(widget): spread grid/battery circles to use full card width

## 1.0.323
- feat(widget): replace power grid with SVG flow diagram; add responsive resize

## 1.0.322
- refactor(price): introduce MarketPrice and ContractPrice classes

## 1.0.321
- fix(overview): anchor nodes to their correct screen edges on resize

## 1.0.320
- fix(price): always show market and contract price independently of active source

## 1.0.319
- fix(price): handle Nordpool/Tibber/EPEX sensor attribute formats in price charts

## 1.0.318
- fix(dashboard): market price chart always shows market data, not active source

## 1.0.317
- fix(ems): respect price_source setting when selecting AUTO_BUY/AUTO_SELL mode

## 1.0.316
- fix(control): always show price source dropdown regardless of sell mode

## 1.0.315
- fix(run.sh): add diagnostic logging to companion integration install step

## 1.0.314
- fix(overview): include grid controller battery power in flow display

## 1.0.313
- feat(grid-controller): add battery power visibility and dashboard/overview display

## 1.0.312
- fix(settings): create battery_settings.json on first run if missing

## 1.0.311
- fix(settings): write new default keys back to battery_settings.json on load

## 1.0.310
- fix(savings): replace full-width nav menu with compact dropdown

## 1.0.309
- fix(savings): use relative URL for public_ems_data fetch

## 1.0.308
- fix(ui): move debug refresh controls out of header; improve savings diagnostics

## 1.0.307
- feat: auto-fill inverter power limit companion entities from device name

## 1.0.306
- fix(ui): standardize nav header order, add SOC hysteresis for sell mode, fix savings page data source

## 1.0.305
- fix(ui): replace ventra-icon img tags with inline SVG on all pages

## 1.0.304
- fix(ui): replace img tag with inline SVG for nav icon; add mini widget for website embedding

## 1.0.303
- feat(savings): add daily savings tracker and savings debug page

## 1.0.302
- feat(config): split internal name from friendly_name for display

## 1.0.301
- fix(ui): serve static assets via FileResponse instead of StaticFiles

## 1.0.300
- fix(integration): add icons.json to show MDI icon on HA Integrations page

## 1.0.299
- fix(icon): replace old logo.png with new Ventra-EMS branding

## 1.0.298
- feat: auto-install companion integration and add header branding

## 1.0.297
- fix: always correct companion entity IDs; gate EV/relay animations on is_running; EV take_control is mode-only

## 1.0.296
- feat(ems): rework AUTO_BUY as mirror of AUTO_SELL; add manual buy/sell per-battery rates; route control page through UIPresenter

## 1.0.295
- disable a device fix

## 1.0.294
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.293
- fix(config): fix YAML syntax highlighting for string values

## 1.0.292
- feat(config): auto-fill companion integration entity IDs from device names

## 1.0.291
- docs: document companion HA integration and entity naming convention (§ 14)

## 1.0.290
- feat(ui): add heatpump, relay_load, and AC cards to dashboard and overview

## 1.0.289
- chore: remove unused client setup and public index files

## 1.0.288
- fix(config): add air_conditioners to config validator and align AC YAML style

## 1.0.287
- fix(ems): relay loads always assert EMS control when mode_key participates

## 1.0.286
- fix(devices): enforce negative sign on energy sensors for all load devices

## 1.0.285
- fix(overview): correct Type 2 EV plug icon pin layout

## 1.0.284
- fix(overview): restore EV charger status labels in device circle

## 1.0.283
- fix(devices): always-negative power convention + power display in device nodes

## 1.0.282
- fix(overview): shrink EMS triangles and flip tip to point inward

## 1.0.281
- refactor(sell-schedule): unify trade slot display through UIPresenter

## 1.0.280
- feat(overview): add amber triangle EMS control indicator on device nodes

## 1.0.279
- feat(overview): split relay device status into independent power + EMS control labels

## 1.0.278
- fix(overview): replace CSS animation-duration with JS-driven strokeDashoffset

## 1.0.277
- feat(inverter): add solar power limiting to prevent grid over-export

## 1.0.276
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.275
- fix(overview): EV charger icon — bottom 2 circles same size as middle 3

## 1.0.274
- feat(overview): smooth flow-line animation speed transitions via RAF lerp

## 1.0.273
- fix(overview): sell tick transparent at current SoC when no trade window

## 1.0.272
- style(overview): rationalise sell card font sizes

## 1.0.271
- fix(overview): restore home circle neutral colour; remove diagnostic blue

## 1.0.270
- fix(overview): hoist tickSoc out of if(hasBat) block to fix ReferenceError

## 1.0.269
- test(overview): turn home circle blue to verify page updates are live

## 1.0.268
- revert(main): remove force-gzip serving, restore FileResponse for HTML pages

## 1.0.267
- fix(overview): restore device energy below circle; remove HTML caching

## 1.0.266
- fix(main): force-gzip HTML pages to bypass HA nginx Accept-Encoding strip

## 1.0.265
- fix(main): gzip compress all HTTP responses to avoid nginx proxy buffer overflow

## 1.0.264
- fix(main): prevent partial page loads through HA ingress nginx proxy

## 1.0.263
- feat(ev-charger): add energy_entity support; move device energy inside ring

## 1.0.262
- fix(overview): sell tick shows projected post-sell SoC, not static floor

## 1.0.261
- refactor(dashboard): unify sell schedule card with overview page

## 1.0.260
- fix(dashboard): restore contract price display and chart data

## 1.0.259
- fix(overview): sell strategy card — show hours not year, fix title casing

## 1.0.258
- fix(overview): replace SSE with 2s polling for reliable multi-device support

## 1.0.257
- fix(overview): watchdog reconnects stuck SSE connections automatically

## 1.0.256
- fix(overview): eliminate false OFFLINE flashes on tab switch / page return

## 1.0.255
- feat(overview): scale grid line color and animation below balanced threshold

## 1.0.254
- fix(public): serve overview.html from same dir as backend; remove REPO_DIR

## 1.0.253
- feat(public): make root route serve overview.html instead of old dashboard

## 1.0.252
- chore: exclude deploy_backend.py from git (contains credentials)

## 1.0.251
- fix(deploy): handle socket.timeout + use venv python path directly

## 1.0.250
- fix(deploy): prevent SSH channel hang during process start

## 1.0.249
- fix(deploy): correct deploy order + single file + hard verify

## 1.0.248
- feat(deploy): add backend deploy script for Proxmox LXC

## 1.0.247
- feat(overview): battery SoC ring smooth color + sell floor tick

## 1.0.246
- feat(overview): grid left-fade extension line

## 1.0.245
- feat(overview): consistent circle layouts, Inter font, tabular-nums

## 1.0.244
- fix(heatpump,relay_load): use abs() for idle power threshold check

## 1.0.243
- feat(overview): solar label right-of-ring via JS, wider sell card, bigger sell fonts

## 1.0.242
- feat(overview): move Solar label to the right of the circle

## 1.0.241
- fix(overview): fix connector line gaps + rename Sell Window → Sell Strategy

## 1.0.240
- feat(overview): sell card — move up, add source/threshold header, sort by time

## 1.0.239
- fix(price): use contract_price_sensor attributes when no separate forecast sensor configured

## 1.0.238
- test(grid-controller): add gc_simple + gc_mixed fixture configs and tests

## 1.0.237
- feat(grid-controller): add GridController device type

## 1.0.236
- feat(overview): sell window card above grid node

## 1.0.235
- feat(overview): user-friendly EV status labels in overview nodes

## 1.0.234
- fix(companion): restore number state via RestoreEntity not RestoreNumber

## 1.0.233
- fix(companion): use RestoreNumber for number entities

## 1.0.232
- feat: wire /api/required_entities from config + migrate inverters.yaml to switch/number domains

## 1.0.231
- feat(poc): companion integration + domain-aware control routing

## 1.0.230
- fix: log configuration.yaml snippet when helper auto-creation fails

## 1.0.229
- fix: correct HA helper creation URL — POST to collection, id in body

## 1.0.228
- test: add power_entity and energy_entity to relay load in full_house fixture

## 1.0.227
- fix: helper creation — remove id from JSON body, fix misleading log message

## 1.0.226
- fix(overview): display power as NNN W below 1 kW, N.N kW above

## 1.0.225
- refactor: remove pv_power_entity_invert and pv_yield_entity_invert

## 1.0.224
- feat(overview): home circle color reflects load/mode/offline state

## 1.0.223
- fix(overview): battery lines orange when charging, green when discharging

## 1.0.222
- feat(public): update public page, overview and backend to UIPresenter snapshot format

## 1.0.221
- fix(ui_presenter): restore forecast graph data for market price source

## 1.0.220
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.219
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.218
- fix(overview): increase text size in solar and battery mini circles

## 1.0.217
- fix(overview): force SSE reconnect on page visibility change

## 1.0.216
- feat(overview): green grid line on export + grid load arc ring

## 1.0.215
- fix(overview): prevent flow-line track brightening where lines overlap

## 1.0.214
- fix(overview): move bottom device circles up by 1/8 of screen height

## 1.0.213
- feat(overview): inverter max power config + solar arc + layout fixes

## 1.0.212
- fix(overview): debounce offline indicator to hide transient SSE drops

## 1.0.211
- fix(overview): unify and reduce glow highlight on all circle nodes

## 1.0.210
- fix(overview): spacing, battery line color, and solar yield label tweaks

## 1.0.209
- fix(overview): fix 5 layout/animation issues in energy flow diagram

## 1.0.208
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.207
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.206
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.205
- feat(overview): correct price source in grid node + add per-inverter solar mini-nodes

## 1.0.204
- fix(overview): move home row to 3/8 of screen and fix mini-battery path direction

## 1.0.203
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.202
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.201
- center home vertically; mini batteries at midpoint between solar and battery

## 1.0.200
- dynamic ring and font sizes: enforce minimum visual diameter per screen

## 1.0.199
- remove top status card; mode→home circle, price→grid circle; full-screen layout

## 1.0.198
- fix sub-battery animation jitter and off-screen clipping

## 1.0.197
- redesign overview page with larger nodes and all data in animation

## 1.0.196
- update the overview page

## 1.0.195
- Merge pull request #2 from frank8the9tank/claude/earnings-whole-day-calc-o3z08d

## 1.0.194
- feat(overview): show whole-day potential earnings in the stats strip

## 1.0.193
- feat(control): potential earnings now reflect the whole day (past + future), planned sell windows unchanged

## 1.0.192
- feat(overview): animated sub-lines from aggregate battery to mini-nodes

## 1.0.191
- fix(overview): move battery mini-nodes to top-right, spread left

## 1.0.190
- refactor(control): move earnings calculation to backend

## 1.0.189
- feat(control): show potential earnings in sell windows panel

## 1.0.188
- Merge branches 'main' and 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.187
- feat: add test suite, mock HA server, and CI

## 1.0.186
- feat: show individual battery mini-nodes on overview page

## 1.0.185
- revert: remove Docker image build from CI and image key from config.yaml

## 1.0.184
- fix: use lowercase recovery_power_kw attribute on EVCharger (was RECOVERY_POWER_KW)

## 1.0.183
- feat: pre-build Docker images to GHCR so HA pulls instead of building locally

## 1.0.182
- fix: create EVChargerStatusSensor directly, not via _make_sensor (no sign/invert needed)

## 1.0.181
- fix: EVChargerStatusSensor missing sign/invert params from base Sensor class

## 1.0.180
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.179
- 

## 1.0.178
- 

## 1.0.177
- changed more default values

## 1.0.175
- fix: guard against None price sensor in _select_mode and _determine_sub_mode

## 1.0.173
- changed default values

## 1.0.171
- feat: add EN/NL language toggle to overview page

## 1.0.170
- style: standardise font and CSS tokens across all pages

## 1.0.169
- docs: add inverters.yaml schema versioning and migration design

## 1.0.168
- style: remove 'left' from battery capacity label on overview page

## 1.0.167
- feat: replace horizontal nav with hamburger menu across all pages

## 1.0.166
- style: larger nodes and labels on overview flow diagram

## 1.0.165
- feat: add EMA smoothing toggle to overview page

## 1.0.164
- fix: smooth flow animation by updating SVG paths in-place

## 1.0.163
- feat: light/dark theme for overview and schedule pages, remove SOC arc

## 1.0.162
- fix: unified nav header and mobile-friendly overview page

## 1.0.160
- implement Phase A device scheduling system

## 1.0.158
- add Overview landing page and device scheduling design

## 1.0.156
- added heatpump and relay devices to the EMS code base

## 1.0.154
- sign changes and ev reconnect logic after auto sell

## 1.0.153
- changes to power share calculation

## 1.0.151
- public link is restored

## 1.0.149
- pricing changes

## 1.0.148
- changed sensor to read for grid power data

## 1.0.147
- changed default config for clean install

## 1.0.146
- updated build routine for home assistant green

## 1.0.144
- price table fixes

## 1.0.142
- more price table fixes

## 1.0.141
- update github actions

## 1.0.140
- more coloring changes

## 1.0.139
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.138
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.137
- changed color schema for price information

## 1.0.136
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.135
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.134
- more fixes for flow page

## 1.0.133
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.132
- more fixes for ev charger sign

## 1.0.131
- updated flow page

## 1.0.130
- corrections for ev charger sign

## 1.0.129
- quick fix for stupid me.......

## 1.0.128
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.127
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.126
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.125
- more restructuring

## 1.0.124
- ev charger rework

## 1.0.123
- more fixes for ev charger disconnecting

## 1.0.122
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.121
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.120
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.119
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.118
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.117
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.116
- simpler logic for ev charging

## 1.0.115
- more fixes for charging control

## 1.0.114
- fix for not enableling the inverter in standalone mode

## 1.0.113
- added functions to start ev charging form the EMS

## 1.0.112
- add minimum disharge level for inverters

## 1.0.111
- moved the control EMS enable to other page

## 1.0.110
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.109
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.108
- restructuring of sensors and headers

## 1.0.107
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.106
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.105
- changed page width

## 1.0.104
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.103
- greyed out for manual mode

## 1.0.102
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.101
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.100
- add minimum SOC for sell mode

## 1.0.99
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.98
- fix for absorbed state calculation

## 1.0.97
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.96
- changed graph data to a single url

## 1.0.95
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.94
- more general fixes for publishing

## 1.0.93
- fix for popup box not scrolling with the page

## 1.0.92
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.91
- Merge branches 'main' and 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.90
- more display issues

## 1.0.89
- changes for prices cards

## 1.0.88
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.87
- Merge branches 'main' and 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.86
- styling changes

## 1.0.85
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.84
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.83
- graph changes

## 1.0.82
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.81
- add level system to show/hide cards and data

## 1.0.80
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.79
- Merge branches 'main' and 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.78
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.77
- add debug page

## 1.0.76
- more fixes

## 1.0.75
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.74
- fix for ev charger setpoint to home assistant

## 1.0.73
- fix for not displaying ev charger cards

## 1.0.72
- add ev charger to yaml file

## 1.0.71
- added different logic for maximum export

## 1.0.70
- added new style of interface

## 1.0.69
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.68
- added a way to restart the internal login

## 1.0.67
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.66
- add changes for export limit

## 1.0.65
- add max export config

## 1.0.64
- changed path for config page

## 1.0.63
- add config editor page

## 1.0.62
- added language function for english and dutch

## 1.0.61
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.60
- fix to wrong direction of slew rate

## 1.0.59
- added slowing function for change rate

## 1.0.58
- fix for multi display inputs to EMS

## 1.0.57
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.56
- more diplay fixes for the graphs

## 1.0.55
- cleaner cards

## 1.0.54
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.53
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.52
- added contract price entities, and new graph for contract forecast

## 1.0.51
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.50
- allow to enable and disable an inverter

## 1.0.49
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.48
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.47
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.46
- make control also visable on the public page

## 1.0.45
- fix for 15 minute window, add grid connection size in yaml file

## 1.0.44
- Merge branches 'main' and 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.43
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.42
- more fixes for the graph axis

## 1.0.41
- added changes for graph axis, and removed shadow box in box

## 1.0.39
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.38
- changed balance calculation

## 1.0.37
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.36
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.35
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.34
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.33
- changed color for absorbed state

## 1.0.32
- claude fix for graph not showing data

## 1.0.28
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.27
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.26
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.25
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.24
- changed font size

## 1.0.23
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.22
- changed port number from 8126 to 8125

## 1.0.21
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.20
- still calculate the setpoint even when a inverter is in standalone mode

## 1.0.19
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.18
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.17
- move checks for active mode when to switch between standalone and ems control

## 1.0.16
- added option to control the ems mode per inverter

## 1.0.15
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.14
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.13
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.12
- feat: add index route and improve error handling in data fetching

## 1.0.11
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS-V2

## 1.0.10
- changed config file location

## 1.0.9
- Fix casing in add-on startup message

## 1.0.8
- Update add-on name in run.sh

## 1.0.7
- Update repository name and URL for version 2

## 1.0.6
- Rename public/config.yaml to config.yaml

## 1.0.2
- Merge pull request #1 from frank8the9tank/new-refactoring

## 1.0.1
- typo

## 1.0.77
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.76
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.75
- moved the battery state indicator

## 1.0.74
- fix for formatting error

## 1.0.73
- added charge and discharge indicator

## 1.0.72
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.71
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.70
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.69
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.68
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.67
- added port mapping

## 1.0.66
- change logic for selling energy

## 1.0.64
- changed logic for solax inverter

## 1.0.63
- changed threshold to vertical bar

## 1.0.62
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.61
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.60
- added absorbed state to control logic

## 1.0.56
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.55
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.54
- fix for last update, too many values to unpack

## 1.0.53
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.52
- card collapsable

## 1.0.51
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.50
- added dev mode option to show more information

## 1.0.49
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.48
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.47
- fixes

## 1.0.46
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.45
- logic change

## 1.0.44
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.43
- changes to logic

## 1.0.42
- mode auto mode fixes

## 1.0.41
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.40
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.39
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.38
- fixed rearrenging things

## 1.0.37
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.36
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.35
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.34
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.33
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.32
- changed spacing things

## 1.0.31
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.30
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.29
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.28
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.27
- add sharing code when battery is empty

## 1.0.26
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.25
- added a graph

## 1.0.24
- add entity with dynamic pricing information

## 1.0.23
- Merge branches 'main' and 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.22
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.21
- changed naming for modes on webpage

## 1.0.20
- removed shadow box

## 1.0.19
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.18
- changed the weighing between the batteries

## 1.0.17
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.16
- formating for input boxes

## 1.0.15
- add input boxes for settings forced control values

## 1.0.14
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.13
- removed config.json

## 1.0.12
- Merge branch 'main' of https://github.com/frank8the9tank/Ventra-EMS

## 1.0.11
- added auto version number for config.yaml

## 1.0.10
- removed the ev functions

## 1.0.9
- changes for auto versioning

## 1.0.8
- changed terminal logging based on config entry

## 1.0.7
- added code to auto update then changelog

## 1.0.x
- Automated versioning and bug fixes.
- Integrated price-based battery control logic.