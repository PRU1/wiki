---
Link: https://digitalcommons.usu.edu/cgi/viewcontent.cgi?article=5247&context=smallsat
---
FINCH: A Blueprint for Accessible and Scientifically Valuable Remote Sensing Missions

Adyn Miles, David Maranto, Shiqi Xu, Rosalind Liang, Yong Da Li, Jason Rock, Amreen A. Imrit, Maggie Kou, Abeer Fatima, Allen Kasum, Amy Saranchuk, Ana-Maria Zamrii, Andy Gong, Angelina Hui, Anthony DiMaggio, Benjamin Nero, Bettina Oghinan, Bruno Almeida, Brytni Richards, Cameron

Rodriguez, Dhruv Sirohi, Eman Shayeb, Emma Belhadfa, Eren Cimentepe, Erie Wu, Ginny Guo, Harshit Sohaney, Hiba Al-Falahi, Ian Vyse, Iliya Shofman, Jasnoor Guliani, Jennifer Zhang, Kanver Bhandal, Kejsi Gjerazi, Ketan Vasudeva, Khalil Damouni, Kimberley Orna, Konstantinos Papaspyridis, Kyoka Collina

Stone, Maggie Fen Wang, Mary Cheng, Maxime Michet, Mingde Yin, Mirai Shinjo, Nicholas Glenn, Novera Ahmed, Omar Farag, Prachi K. Sukhnani, Punyaphat Sukcharoenchaikul, Rajvi Rana, Rediet Yohannes, Selena Liu, Shuhan Zheng, Stephanie Yi Fei Lu, Tianyi Zhang, Tobias Rozario, Wanda Janaeska, Yifan

(Julia) Ye, Ziyu Chen

University of Toronto Aerospace Team 4925 Dufferin St, Toronto, ON; 416-317-1266

adynmiles.am@gmail.com

ABSTRACT

Satellite remote sensing missions have grown in popularity over the past fifteen years due to their ability to cover large swaths of land at regular time intervals, making them suitable for monitoring environmental trends such as greenhouse gas emissions and agricultural practices. As environmental monitoring becomes central in global efforts to combat climate change, accessible platforms for contributing to this research are critical. Many remote sensing missions demand high performance of payloads, restricting research and development to organizations with sufficient resources to address these challenges. Atmospheric remote sensing missions, for example, require extremely high spatial and spectral resolutions to generate scientifically useful results. As an undergraduate-led design team, the University of Toronto Aerospace Team’s Space Systems Division has performed an extensive mission selection process to find a feasible and impactful mission focusing on crop residue mapping. This mission profile provides the data needed to improve crop residue retention practices and reduce greenhouse gas emissions from soil, while relaxing performance requirements relative to many active atmospheric sensing missions. This is accompanied by the design of FINCH, a 3U CubeSat with a hyperspectral camera composed of custom and commercial off-the-shelf components. The team’s custom composite payload, the FINCH Eye, strives to advance performance achieved at this form factor by leveraging novel technologies while keeping design feasibility for a student team a priority. Optical and mechanical design decisions and performance are detailed, as well as assembly, integration, and testing considerations. Beyond its design, the FINCH Eye is examined from operational, timeline, and financial perspectives, and a discussion of the supporting firmware, data processing, and attitude control systems is included. Insight is provided into open-source tools that the team has developed to aid in the design process, including a linear error analysis tool for assessing scientific performance, an optical system tradeoff analysis tool, and data processing algorithms. Ultimately, the team presents a comprehensive case study of an accessible and impactful satellite optical payload design process, in hopes of serving as a blueprint for future design teams seeking to contribute to remote sensing research.

INTRODUCTION

Effective environmental monitoring is crucial to the development of sustainable climate strategies. In recent years, the ongoing development of hyperspec- tral remote sensing satellites—particularly smaller, more affordable nanosatellite imaging platforms— has become a cornerstone to furthering this cause.

In accordance with our goals to undertake feasi- ble and scientifically valuable satellite missions, the University of Toronto Aerospace Team’s (UTAT) Space Systems Division is designing and launch- ing FINCH, a 3U nanosatellite with a hyperspec- tral spectrometer payload imaging in the shortwave infrared (SWIR) region of the electromagnetic spec- trum. FINCH’s 3U platform is ideal for a student

Miles 1 36th Annual Small Satellite Conference

team because there is sufficient volume to host a sci- entifically valuable payload while keeping costs man- ageable.

The optical payload, named the FINCH Eye, will be built from a composite of off-the-shelf and cus- tom components, to advance upon the performance achieved by other remote sensing nanosatellite pro- grams with similarly limited budget and expertise. This paper will discuss optical design, optomechan- ical design, and assembly, integration, and testing (AIT) concerns. It will also detail supporting sub- systems for the FINCH Eye, including imaging elec- tronics and firmware, payload operations, and data processing.

Hyperspectral remote sensing allows for the re- trieval of atmospheric concentrations of molecules from the absorption features present in their ab- sorption spectra. In doing so, enhancements, or lo- calized increases in atmospheric concentrations near an emission source, of specific greenhouse gases (GHGs) can be measured. As a substantial emitter of methane (CH4), a potent GHG, municipal land- fills represent one such source for which monitoring becomes crucial, and as such, were investigated as an original mission concept for FINCH. From spec- tral absorption features of carbon dioxide (CO2) and CH4 found near 1600 nm, the proxy retrieval method as described by Frankenberg et al. can be used to extract the column dry air mole ratio of methane (XCH4) over landfills, from which emissions can be derived.1

A previous design iteration revealed that the FINCH Eye would fall short of the spectral resolu- tion typical of CH4 missions (better than 1 nm) due to physical constraints brought on by the small form factor. This meant that it would be unable to dis- tinguish features in the absorption spectrum which are finer than 1 nm apart. To verify whether the proposed payload design could sufficiently resolve XCH4 enhancements over sources of interest, lin- ear error analysis (LEA) was undertaken, the details of which are described in the Linear Error Analysis section. LEA results indicated that the necessary signal-to-noise ratio (SNR) and spectral resolution for a CH4 sensing mission were outside the feasible performance range of the FINCH payload. As a re- sult, the mission was rescoped to lie within design constraints while still providing scientific value.

In the agricultural practice of crop residue reten- tion, residue from a previous harvest is retained in certain fields to reduce the amount of GHG emis- sions from the soil. In order to implement this prac- tice and measure its efficacy, accurate mapping of crop residue coverage is essential. However, histor-

ical methods such as census surveys and roadside measurements capture an insufficient level of spatial and temporal detail.2 To this end, the use of satellite remote sensing provides a much more efficient and robust solution. This mission profile relaxes SNR and spectral resolution requirements from those of a methane sensing mission to be more feasible for an amateur nanosatellite design. The FINCH payload is thus in the process of being adapted to accommo- date this new mission profile, discussed further in the Future Work section.

FINCH is the second mission in UTAT Space Systems’ undergraduate student-led and -funded nanosatellite development program. The team seeks to grow the technical knowledge and leadership skills of undergraduate students through challeng- ing projects with tangible benefits. The team also strives to improve the accessibility of useful aerospace projects by generating open-source de- signs at an undergraduate expertise level. This pa- per will outline FINCH’s mission scoping and instru- mentation design processes, as well as anticipated future work.

RELATED WORK

This section will investigate existing research and projects focused on comparable satellite payloads, remote sensing mission design, and compact spec- trometer optical design.

Satellite Missions

Satellites have been used for remote sensing ap- plications since the development and launch of Land- sat by NASA in 1972.3 Since then, efforts have been made to advance payloads to image the Earth with better spatial, spectral, and temporal resolutions. There has also been significant attention towards miniaturizing these payloads and building constella- tions of satellites for cheaper and more flexible data collection.

NASA’s Landsat was a pioneer for the remote sensing satellite field through its use of a whiskb- room camera for imaging.3 The transition to Cube- Sats for remote sensing applications brought on by Aalborg University through the AAU-CubeSat was also a significant leap.4 The University of Tokyo’s PRISM satellitle made efforts to simplify and shrink the remote sensing system for more prac- tical use in small satellite platforms.5 The Univer- sity of Toronto Space Flight Laboratory’s CANX- 2 3U nanosatellite also contains a spectrometer payload as a technological demonstration.6 Re-

Miles 2 36th Annual Small Satellite Conference

mote sensing performance improved tremendously with the advent of hyperspectral camera technol- ogy, most notably in ESA’s SCIAMACHY System,7

ASI’s PRISMA,8 JAXA’s GOSAT,9 the Nether- lands’ TROPOMI system,9 and ISRO’s HySIS.10

However, these platforms are massive, weighing be- tween 200–1750 kg. Despite high spectral resolution performance across multiple bands, the spatial reso- lution performance of these satellites is on the order of multiple kilometres. More recently, higher per- formance small satellites with improved spatial and spectral resolution have been developed by Planet through their Dove constellation with a spatial res- olution of 3–4 m,11 as well as GHGSat’s GHGSat-D with a spectral resolution of 0.1 nm.12 Not only has the performance improved, but the accessibil- ity of these satellite platforms for teams with fewer resources and less expertise has emerged through MeznSat13 and SathyabamaSat,14 two university- developed nanosatellites carrying spectrometer pay- loads for greenhouse gas emissions research with spectral resolutions around 6 nm and spatial reso- lutions around 1 km.

It is clear that more accessible designs tend to sacrifice significant performance, a gap that FINCH’s design seeks to fill with its open-source platform. FINCH provides an improved balance be- tween the accessibility of the design and its scien- tific usefulness through improved spectral and spa- tial performance. Its spatial resolution even offers an advantage over that of well-established hyperspec- tral systems such as GOSAT and TROPOMI.

Atmospheric Sensing of Methane

Many previous hyperspectral satellite missions which monitor methane, such as EnMAP15 and PRISMA,8 have focused on the strong CH4 absorp- tion features at 2300 nm. This feature is highly conducive to retrieval due to its pronounced absorp- tion of light by CH4 molecules, allowing low mea- surement error to be achieved with spectral resolu- tions as coarse as 5–10 nm. However, this comes with a caveat of increased susceptibility to interfer- ence from surrounding spectral features belonging to other species.16

Other missions such as JAXA’s GOSAT have in- stead made use of moderate absorption features at 1650 nm,17 which requires the proxy method for re- trieving methane column concentrations.1 Although this band has lower sensitivity to instrument perfor- mance issues such as radiometric errors and stray light, it requires finer spectral resolution to resolve methane features than the strong band.16

These challenges make it difficult for low-cost

nanosatellite programs to design imaging payloads geared towards the atmospheric sensing of methane, and have required FINCH to divert its scientific ob- jective to suit a more feasible design.

Crop Residue Mapping

To date, many remote sensing studies on crop residue mapping have used spectral indices to quan- tify percent residue cover. Notable examples in- clude the Normalized Difference Vegetation In- dex (NDVI)18 and the Cellulose Absorption Index (CAI).19 However, these methods are limited by their dependence on absorption features at very spe- cific wavelengths, which often cannot be feasibly im- aged by satellites designed for large area monitor- ing.2

An alternative method for quantifying percent residue cover is Spectral Mixture Analysis (SMA), which uses endmembers, pure spectra of specific land features selected directly from image data, to ex- tract the relative abundance of each endmember in each image pixel.20 Currently, much of the research on SMA for satellite crop residue mapping has in- volved multispectral sensors, such as the Advanced Wide Field Sensor (AWiFS).21 It is hypothesized that SMA performance would be enhanced by hy- perspectral data due to the higher number of spec- tral bands available for classifying each endmember. Thus, there is a need for more hyperspectral satel- lite data to assess its effectiveness at estimating crop residue percent cover via SMA. This makes crop residue mapping an optimal niche for the FINCH mission to fill by supplying the hyperspectral data necessary to validate hypotheses from literature.

Optical Designs

Grism-based spectrometers have seen use in land, air, and space domains. A spectrometer in this context is used to refer to a hyperspectral imager. A grism is an optical element which sandwiches a diffraction grating between two prisms. The combi- nation of these components enables the wavelength of interest to remain centered in the optical axis. At the time of writing, the Technology Readiness Level (TRL)—according to NASA’s designation22—of this type of optical system is a Level 9. Grism-based spectrometers have flight heritage through successful space mission operations.23,24 However, CubeSat- form factor, grism-based pushbroom spectrometers are at a Level 6. Pushbroom spectrometers refer to those that scan the ground target one across- track line at a time, using the orbital motion of the satellite, and incorporating active slewing. Grism-

Miles 3 36th Annual Small Satellite Conference

based pushbroom spectrometers have yet to be de- ployed in a space environment, but have seen use in land-based telescopes and have been tested in aerial vehicles.25–27 Another major goal for FINCH will be to advance the TRL of such optical sys- tems to a Level 9 through the design, deployment, and successful end-to-end mission operation of the first CubeSat-compatible Volume Phase Holographic (VPH) grism-based pushbroom spectrometer. VPH gratings are a diffracting element composed of a dichromate gelatin (DCG) film sandwiched between two substrates. They surmount many of the draw- backs associated with conventional diffraction grat- ings, delivering significantly higher efficiency, greater dispersion, and better polarization characteristics in a robust package.

Ludovici et al. (2017) designed and built a low- cost, low-resolution, compact, in-line, slitless, grism- based spectrometer for use with small astronomi- cal telescopes.25 A slitless spectrometer can only be used to image point sources. It was constructed us- ing commercial off-the-shelf (COTS) optical compo- nents. The Ludovici system consists of five elements: a transmission grating, two achromatic lenses for col- limating and refocusing, and two wedge prisms. It was designed to image in the the visible (VIS) spec- trum (400 to 800 nm).

Kashiwagi et al. (2004) designed and fabricated several large (110×106mm2) VPH grisms for the Faint Object Camera and Spectrograph (FOCAS) of the Subaru Telescope.28 The authors searched for the optimal parameters such as grating thick- ness and strength of the refractive index modulation to achieve high-performing grism designs.

Hyvärinen et al. (2011) designed and built a compact grism-based pushbroom spectrometer pro- totype to be flown on unmanned aerial vehicle (UAV) platforms. It was capable of imaging the vis- ible and near-infrared (VISNIR) spectrum, 350 to 1000 nm, with a spectral resolution of 3 nm. The optical design made use of both transmissive and reflective optics to produce an off-axis design that achieved high light throughput and large spatial im- age size (as formed on the sensor) in a compact for- mat. The prototype achieved an SNR of 800. The imager weighed in at 1.4 kg, including fore-optics and the imaging spectrograph with shutter and cam- era. The proposed system was validated in a flight test mission using a piloted aircraft.

Volent et al. (2017) designed and built a pushb- room spectrometer for conducting airborne kelp for- est mapping.27 It was capable of imaging in the VIS spectrum (425 to 825 nm) at a spectral resolu- tion of 5 nm. The battery-powered, energy-efficient

spectrometer weighed 680 g. It was designed with a front focusing lens, entrance slit with the slit direc- tion perpendicular to the flight direction, collector lens, grism, and silicon CCD detector with a reso- lution of 360 by 280 pixels fitted with a 50mm lens. The system was flown onboard an aircraft to acquire ocean colour data.

The Wide Field Camera 3 (WFC3) is an ultraviolet-visible-infrared (UVISIR) spectrometer installed onboard the Hubble Space Telescope in 2009. WFC3 provides two imaging channels: (1) an ultraviolet-visible (UVIS) channel with sensitivity from 200 to 1000 nm, and (2) an infrared (IR) chan- nel covering 850 to 1700 nm.23 The WFC3 UVIS channel also offers a large and diverse filter set, in- cluding 62 filter elements and one ultraviolet (UV) grism. The WFC3 IR channel contains 15 filters and two grism elements.

The James Webb Space Telescope (JWST) near- infrared camera (NIRCam) contains two grisms with a resolvance of 1500 that can used for slitless spec- troscopy over the mid-wavelength infrared (MWIR) 2400 to 5000 nm spectral range.24 Resolvance is de- fined as the spectral wavelength of interest divided by the spectral resolution.

Table 1 summarises the characteristics of the aforementioned systems.

Summary of Contributions

The FINCH mission seeks to contribute the fol- lowing to the field of remote sensing:

- Open-source the design process of a CubeSat that can successfully take hyperspectral im- ages, increasing accessibility for undergraduate teams.
- Design, verify, and launch the first grism-based pushbroom spectrometer onboard a CubeSat.
- Publish processed hyperspectral data to verify literature results related to SMA for the pur- pose of improving crop residue retention prac- tices.

MISSION SCOPING

Mission scoping is the process of continuously balancing desired scientific objectives and engineer- ing constraints. Unlike traditional mission incep- tions from science proposals, undergraduate teams often begin with the goal of building a nanosatel- lite and must endeavour to unearth a fitting mission concept that can then guide further spacecraft de- sign. As one such undergraduate design team with limited expertise and resources, the mission scoping

Miles 4 36th Annual Small Satellite Conference

Table 1: Value Proposition Comparison Across Grism-Based Spectrometer Reference Designs

Characteristic FINCH Eye Ludovici Kashiwagi Hyvärinen Volent Hubble WFC3 JWST NIRCam

Domain Space Land Land Air Air Space Space Compact ✓ ✓ ✕ ✓ ✕ ✕ ✕ In-line ✓ ✓ ✓ ✕ ✓ ? ? Pushbroom (slit) ✓ ✕ ✓ ✓ ✓ ? ✕ SWIR ✓ ✕ ✕ ✕ ✕ ✓ ✕ VPH ✓ ✕ ✓ ✕ ✕ ✕ ✕ COTS ✓ ✓ ✕ ✕ ✕ ✕ ✕

process for the FINCH mission has involved multiple iterations of research, consultation, and adaptation, before ultimately converging on a mission and a de- sign that balances scientific usefulness with technical feasibility.

Initial scientific mission propositions with the po- tential of being realised by a 3U CubeSat were teased out of literature reviews as well as conversations with experts in various remote sensing niches. A holistic analysis of the feasibility and scientific value of each mission profile was undertaken to select a mission for FINCH. The feasibility portion of this analysis was conducted by assessing the viability for other subsys- tems and ruling out missions that required infeasible designs from any subsystems, then selecting the mis- sion profile that is most achievable for every satel- lite subsystem. This process necessitated significant upfront research to determine what was achievable by each subsystem and where additional innovation would be required. A few key criteria were assessed to determine feasibility, including:

- Cost: FINCH has a limited budget, so op- tions that require more costly components of over $10,000 CAD are considered less feasible.
- Design Timeline: Since the FINCH team has limited expertise, the learning required will lengthen a design cycle. Elements of the design should not take years to learn, as the launch timeline is on the order of a few years.
- Volume: FINCH is restricted to a 3U form factor based on financial constraints, meaning the design cannot introduce components that are too large.
- Image Quality: Since FINCH is small, the amount of light reaching the sensor needs to be maximized. This makes beam-splitting de- signs, or the introduction of too many optical surfaces, less feasible.
- Precedence: For design timeline considera- tions, if a large portion of the design has never been accomplished, it is less feasible that a stu- dent team would be able to do it.

As these bounds vary from mission to mission, mission progress can be stalled during the scoping process. It is therefore advisable to begin early in establishing mission requirements that allow design work to commence. Starting mission scoping and high-level payload design 1 to 2 years before detailed design of the supporting subsystems will minimize design bottlenecks for the entire spacecraft.

The usefulness portion of the analysis included a few key evaluation criteria:

- Hyperspectral Imaging: How necessary is hyperspectral data, as opposed to multispec- tral data?
- Satellite Imaging: How necessary is satel- lite imaging, as opposed to airborne imaging or ground monitoring?
- Technological Advancement: How much would the satellite built to address the chosen mission advance remote sensing technology?
- Scientific Advancement: How much would the chosen mission advance its scientific field?
- Mission Lifetime: How quickly can the mis- sion provide useful trends and actionable out- comes?

These criteria were evaluated in order to deter- mine the quality of each mission from a holistic per- spective, then defined with the feasibility analysis to choose an overall mission preference.

Requirements were derived from the chosen mis- sion, which guided the iteration of payload design that ensued. Payload parameters from that itera- tion were then tested using an in-house tool that evaluated the performance of the proposed design in attaining the scientific objectives of the selected mis- sion profile. This information then guided the next iteration of payload design. This mission scoping feedback process is visualized in Figure 1.

In general, should the existing payload design iteration fail the scientific objectives, the existing mission profile can be descoped or pivoted to a new one that is, for the most part, non-intrusive to exist- ing high-level design parameters. While counterintu- itive to the overarching scientific drive behind UTAT

Miles 5 36th Annual Small Satellite Conference

Space Systems, this constraint helps anchor feasibil- ity of the new mission requirements when translated to the next iteration of technical design. This design workflow was clear through the transition from the methane monitoring mission to one focused on crop residue mapping as described in the Linear Error Analysis section.

Figure 1: Mission Scoping Process.

MISSION PROFILE: METHANE MONI- TORING

After much research, the team’s early interest in a spaceborne greenhouse gas monitoring mis- sion crystallised in the selection of methane as the molecule of interest, imaged in the SWIR band. Methane is known for its considerable impact on global warming, and yet existing inventories of methane concentrations often contain large discrep- ancies.29–32 Key emitters of methane include land- fills (active and buried), waste management sites, and natural gas pipelines and stations.33 Upon

detection of an emission source such as a natural gas leak, mitigation and/or recapture efforts are of- ten practical and highly warranted. The Greater Toronto Area (GTA) is itself home to a number of high methane emitters including landfills as well as compressor stations.34 As such, the initial scien- tific objective of FINCH was to monitor atmospheric CH4 enhancements over GTA landfills.

The strong CH4 absorption features at 2300 nm and moderate features at 1650 nm correspond to the SWIR range. The section of the SWIR spectrum be- tween 900 nm and 1700 nm was deemed feasible for FINCH’s form factor, budget, and component avail- ability. A spectral range of 1600–1680 nm targeting the 1650 nm band was selected, with in mind a proxy retrieval of XCH4 utilising the nearby CO2 feature at 1610 nm. Designing for fine spectral resolutions of 1 nm or less is recommended by literature in order to guarantee adequate resolution of necessary features for XCH4 retrieval, suggesting that the spectral res- olution of the FINCH Eye should be refined to the fullest extent possible.16

To facilitate the capture of multiple landfills in one scene, a swath of at least 50–100 km is recom- mended.35 Additionally, a spatial resolution on the order of 100 m would enable the resolution of point sources, and would be an improvement upon exist- ing methane-monitoring satellite platforms such as TROPOMI and GOSAT.369 These imaging systems have the favoured global coverage at the expense of spatial resolution, which falls on the order of a few kilometres.

Table 2: Key Requirements for the Methane Monitoring Mission

Parameter Anticipated Requirement

Spectral Range 1600–1680 nm

Spectral Resolution < 1 nm

Spatial Resolution 100 m

Swath 50-100 km

Mission Lifetime 1 year

Table 2 summarises the scientific requirements derived from the methane mission profile. While the mission profile was later determined to be infeasible from the analysis outlined in the LEA section, the following sections discuss the current iteration of the payload design made to accommodate this mission. Many design principles will carry forward to future iterations of the FINCH Eye. The design changes necessitated by the switch to crop residue mapping are discussed in the Future Work section.

Miles 6 36th Annual Small Satellite Conference

FINCH EYE OPTICAL DESIGN

Table 3: FINCH Eye Specifications. Specification Value Units Cost $101,000 CAD Mass <500 g

Dimensions 44 × 44 × 160

mm

Athermal Range −40 to 70 °C Integrated Cooling Yes - Power (max) 3.2 W Voltage 5 V Focal Length 100 mm Aperture diameter 80 mm F-number 2.5 - Field of View (across, along track)

11.42, 0.57 °

Transmission efficiency (average)

60 %

Wavelength range 1600 to 1700 nm Spectral resolution 2 nm Bands (spatial, spectral) 640, 50 - Specific spectral bandwidth

10 px/band

Spectral nonlinearity < ±2 nm Smile Subpixel - Keystone Subpixel -

Straylight Below sensor noise floor

Flare(s) /ghost images None - RMS Spot Diameter <15 µm Polarization sensitivity <2 % Signal-to-noise (average)

85 -

Quantum efficiency (average)

>60 %

Pixel well capacity 19 ke−

Noise TBD ke−

Radiometric resolution 14 bit Radiometric stability < ±2.5 % Non-linearity < 2 % Method Pushbroom - Spatial resolution (500 km)

75 m

Swath (500 km) 100 km Framerate (max) 60 Hz

Datacube dimensions 640 × 640 × 512

px

Datacube size (uncompressed)

368 MB

Duration TBD s Ground track dimensions

48× 48 km

Pointing Constraint (500 km)

TBD °

Slew rate TBD ° s−1

The FINCH Eye is the first compact, low- cost, VPH grism-based pushbroom spectrometer, designed to image the SWIR (1600–1700 nm) part of the electromagnetic spectrum. It leverages custom and commercial off-the-shelf components to reduce costs and development time. Its design is driven by the need for a hyperspectral imager with a spec- tral resolution on the order of 1 nm that fits within FINCH’s form factor. As of its inception, no other commercial all-in-one spectrometers exist that fit within the 3U CubeSat form factor. Table 3 presents

a summary of design specifications.

Key Optical Components

An in-line optical track, enabled by the VPH grism diffraction mechanism, facilitates assembly and integration with the rest of the spacecraft, while reducing the volume of the payload. A custom cata- dioptric fore-optic lens with a wide aperture is used to maximise light throughput. Achromatic doublet lenses are employed in the design to mitigate chro- matic aberrations. A 640 × 512 Indium-Gallium- Arsenide (InGaAs) sensor captures the diffracted SWIR spectra. Figures 2, 3, and 4 show a render- ing of the conceptual model for the payload, while Figure 5 presents a mechanical drawing.

Figure 2: Isometric Figure 3: Side View

Figure 4: Payload in CubeSat Body

Figure 5: FINCH Eye Mechanical Drawing

The FINCH Eye consists of the following seven components:

- Fore-optics: Captures light from the ground target. Employs a catadioptric lens design for a low profile. Bespoke by Chromar Technol- ogy.

Miles 7 36th Annual Small Satellite Conference

- Slit: Selects a row of the image formed by the fore-optics. Reduces the field of view to that of a rectangular scan line across the ter- rain. Coated to reduce stray light. Bespoke by Walthy.
- Collimator: Collimates light for relay into the rest of the optical track. Employs an achromatic doublet lens design to reduce chro- matic aberration. By Edmund Optics.
- Bandpass filter: Blocks all light outside the 1600–1700 nm spectral band to reduce stray light. Employs a dichroic filter substrate for high efficiency. Bespoke by Iridian.
- Grism: Diffracts the light beam into its com- ponent wavelengths. Employs a Volume-Phase Holographic Grating technology for high effi- ciency and prisms to enable an in-line design. Sandblasted on the exterior to mitigate stray light. By Wasatch Photonics.
- Focuser: Focuses the diffracted light onto the imaging sensor. Employs an achromatic dou- blet lens design. By Edmund Optics.
- Sensor: The Tau SWIR camera (discussed below). Captures spatial and spectral infor- mation in the across-track and along-track di- rections, respectively. Incorporates a high- resolution 640 × 512 InGaAs sensor. By Tele- dyne FLIR.

Payload Sensor

The primary type of photosensitive semiconduc- tor used for the SWIR range is InGaAs, for its high sensitivity without the need to be cryogenically cooled, which saves significant volume and mass. Multiple vendors were consulted prior to the selec- tion of the FLIR Tau SWIR sensor core. Other candidate modules could only output data using the Camera Link protocol, which uses a low-voltage dif- ferential signaling (LVDS) physical layer. Although better for signal integrity, this would have required additional transceivers to deserialize the data into a parallel format, unnecessarily increasing design com- plexity. The FLIR Tau provided support for the CMOS parallel image data output format in addi- tion to a Camera Link option, making it the simpler option for development. The FLIR Tau was also the sole candidate to outline thermal shock, mechanical shock, and vibration specifications, which indicate a certain consideration for potential aerospace appli- cations of the product. The FLIR Tau 2, the sister product to the FLIR Tau, has flight heritage aboard the Phoenix 3U CubeSat from Arizona State Uni- versity.37

Throughput and Signal-to-Noise

Every fraction of light matters for an already light-starved application, as is the case with a pas- sive remote sensing, miniature, dispersive platform. Figure 6 illustrates the expected light path through the payload. The design employs stray light mitiga- tion strategies, such as anti-reflective (AR) coatings on the lenses, dark coatings on the housing walls, and high-transmission materials, to minimise light loss.

Figure 6: FINCH Eye Ray Trace Concept

The estimated SNR of the spectrometer across the design spectral range is shown in Figure 7. This estimate was generated using the team’s custom pay- load and system modelling tool, Payload Designer. Code can be found on the Payload Designer GitHub, with full GitHub resources listed at the end of this work.

Figure 7: FINCH Eye Theoretical Signal-to- Noise Performance

Optical Design Trade Analysis

Various trade-offs were considered in the design of the FINCH Eye.

The choice of focal length was driven by a trade between spatial resolution and swath, as shown in Figure 8, generated by the Payload Designer tool. An increasing focal length yields a finer spatial reso- lution, but results in a smaller swath. A focal length of 100mm was chosen to enable a spatial resolution of 80m and across-track swath of 17 km.

Miles 8 36th Annual Small Satellite Conference

Figure 8: Spatial Resolution and Swath Ver- sus Focal Length

OPTOMECHANICAL DESIGN

The optomechanical design is essential in main- taining the position, tolerance, and environmental protection necessary for the high spectral and spa- tial requirements of the FINCH Eye. In particular, the design aims to maximise SNR through the reduc- tion of stray light, precision of mounting interfaces, and stability of structural design. Additionally, the optomechanical design seeks to minimize cost, vol- ume, and mass.

To maintain FINCH’s 3U form factor, the pay- load was constrained to a 1.5U volume envelope and a 1 kg mass budget. The CubeSat Design Specifi- cation Rev. 13 places a mass constraint of 4.00 kg on 3U CubeSats.38 The FINCH Eye’s optomechan- ical design takes advantage of the radial symmetry of key optical components through a modular barrel assembly, threaded into a custom deformable grism enclosure.

Figure 9: A CAD Rendering of the Proposed FINCH Eye Housing

Utilizing modules for each of the optical compo- nents ensures higher assembly and alignment pre- cision.39 A separate barrel module was designed for the slit to achieve tighter angular alignment tol- erance, reducing optical errors. Additionally, the highly compartmentalised nature of this design is

appealing for testing while the optics subsystem op- timizes the spacing and the tolerances between pay- load imaging elements.

The FINCH Eye’s housing is shaped around the anticipated light path to reduce scattering and stray light effects, as shown in Figure 9. As such, the bar- rel geometry was chosen to match the geometry of the lenses, filter, and slit, taking reference from the double-imaging ARCSTONE payload.40 This lever- ages the radial symmetry of the optical design, elim- inating tolerance concerns with clock adjustments, while meeting tight tip and tilt tolerances.

The tubular structure of the housing will be ma- chined with Aluminium 6061-T4 due to its strength, low density, and reliable spaceflight heritage. A black anodized coating will be applied to the pay- load’s internal surfaces to improve heat resistance, radiation protection, and stray light mitigation.41

The structural performance metrics are detailed be- low in Table 4. FOS refers to the factor of safety.

Table 4: Performance Metrics of the Pro- posed FINCH Eye Optomechanical Design

Vol [cm3] Mass [g] Cost [CAD]

16.2 × 5.7 × 3.8 138.56 1724.38

FOS (X) FOS (Y) FOS (Z)

5 5 18

The Z-axis length is limited by the distance be- tween optical elements and the length of the fore op- tics. It is currently just over the volume envelope of the 1.5U requirement, pending optical optimization.

The cost was estimated through the Hubs quote generator42 using CNC machining and anodized sur- face treatment. The use of off-the-shelf retaining rings and an online vendor makes this design widely accessible.

The FOS of the mounting structure was calcu- lated using a quasi-static load of 70.5g, equal to the 5σ value from the GSFC-STD-7000B qualifi- cation for components weighing 22.7 kg or less.43

This load was applied to the optical components and structure, accounting for compressive forces, bend- ing of the barrel flanges, threading failure, and bolt- ing interfaces. The Z-axis limiting FOS is found at the interface between the grism mount and the M3 screws. Both the X- and Y-axis failures occur at the threaded retaining rings. Another particular area of concern is the FLIR Tau sensor, which is cur- rently not rated for the expected launch vibrational loads. The optomechanical design will rely on pas- sive damping through mounting geometry, but care will be taken in simulating and testing the sensor

Miles 9 36th Annual Small Satellite Conference

through environmental conditions, as discussed in the following section.

Figure 10: Cross-sectional View of the Op- tomechanical Structure

The placement of venting holes between modu- lar optical components was inspired by the BRITE telescope satellite.44 The choice of sandwiching op- tical elements between two threaded retaining rings also allows for easier assembly, fine-tuning, and dis- assembly which is valuable during the AIT phase of the mission. The first retaining ring can be threaded to the optical element’s ideal position. The lens will then be inserted, and the second retaining ring will provide the pre-calculated load necessary to keep the element in place during launch.39 A cross-sectional view of this design can be seen in Figure 10.

This design calls for a toroidal sealing interface between the achromatic lenses and the retaining rings with off-the-shelf ThorLabs SM15RR threaded fasteners that will be used during the prototyping phase. This will allow for the precise alignment nec- essary for payload assembly and verification, but may cause excessive contact stresses depending on the radius of curvature of the lenses.45 Detailed de- sign following optical optimization and tolerancing will explore different seal geometries.

Although the interface between the FINCH Eye and the remainder of the spacecraft has not yet been determined, low-thermal conductance, expansion- controlled bipods similar to those used on ASTERIA are currently being explored.46

ASSEMBLY, INTEGRATION, AND TEST- ING

The verification and validation procedures for optical designs can rival the design itself in required financial and timeline resources. The payload should be tested in numerous expected environments, which incurs risk to the payload due to high testing loads or cumulative damage. The testing campaign was therefore developed with a cost-reduction mentality,

choosing the simplest and lowest-risk tests that ver- ify the key performance metrics of the FINCH Eye.

Testing in representative environments is crucial for optics, as small changes in temperature or load can induce major imperfections in the final image. The first representative environment is a thermal vacuum (TVAC) chamber, which emulates the vac- uum and temperature conditions in orbit. By per- forming a series of image quality tests inside a ther- mal vacuum chamber, the expected performance of the FINCH Eye in orbit can be accurately predicted.

Figure 11 shows the testing setup for the im- age quality testing campaign inside a TVAC cham- ber. The Systems PCB in this figure refers to a system-level debugging board developed in-house. This board is connected through wire harnesses de- signed to connect to the spacecraft via interfaces built into the TVAC chamber wall. Using an optical port, tests can be performed that verify simulated and calculated payload performance.

Figure 11: Test Setup for the Thermal Vac- uum Chamber Image Quality Testing Cam- paign

The first image quality test is a spectral accuracy and resolution test, determining how well the pay- load is able to correctly identify an incoming wave- length and resolve it to the expected spectral resolu- tion. It does this by sending in a desired wavelength through a uniform light source, then pivoting the in- coming wavelength around that central wavelength by a few nanometres, measuring how the sensor is re- ceiving the data and changing to accommodate new information.

The second test is for SNR, which is broken into two components. The signal portion of the test sim- ply measures the incoming intensity from a uniform light source. The most important noise contribu- tor, dark noise, can be characterised by covering the optical port of the TVAC chamber and varying the temperature.

Miles 10 36th Annual Small Satellite Conference

The third test is for stray light, and measures spectral and geometric stray light using filtered and skewed light sources, respectively, to ensure that the acceptable limit of unintended light detected by the sensor is not being exceeded.

The final test focuses on the linearity and uni- formity of the response of the sensor itself, which is important for establishing a baseline for future on- orbit calibrations (as described in the Payload Oper- ations and Manoeuvres section) by recording sensor response under varying light source intensities.

A few important systematic errors are captured in this testing campaign, including stray light, flat field effects, and non-linearity. By determining the absolute effect that other systematic errors have on scientific accuracy, further tests can be included or re-prioritized as well. This can be done using the LEA tool.

Figure 12: Illustration of Proposed Vibration Testing Strategy

Another critical environmental test is vibration testing, which evaluates the satellite’s response to launch loads. Launch imparts taxing loads onto the entire satellite, which causes great risk to the deli- cate optical system. A vibration testing campaign was designed to minimize the risk of damaging flight components while still qualifying the payload and the structure for launch. First, an engineering model consisting of mass models and other cheap optical alternatives will be tested above expected launch loads. Next, the flight components will be validated for launch through an acceptance test that is done at the expected launch loads. This test is accompanied by functional testing, which focuses on ensuring that optical alignment and overall image quality are not affected by launch vibrations. There is also an op- portunity to isolate the riskiest launch component, the FLIR Tau SWIR sensor, to reduce some uncer- tainty in functional testing. However, as this does

add additional risk of damaging expensive compo- nents, further evaluation through simulation results must be done before committing to a more complex vibration campaign. Figure 12 shows the proposed vibration campaign.

IMAGING ELECTRONICS AND FIRMWARE

Image Capture and Storage Architecture

The FLIR Tau SWIR sensor outputs 14-bit par- allel data. There are three additional timing signals which are referred to by vendors using multiple equivalent terms. For changing the pixel, the name used is pixel clock. For changing the row, the names used are row clock, line valid, or horizontal sync. For changing the frame, the names used are frame sync, frame valid, or vertical sync. Figure 13 shows a timing diagram for the parallel output camera. Pixel data is transferred in a grid-wise manner from left-to-right, top-to-bottom. On each pixel clock cycle, the 14 data lines communicate the bit infor- mation for the individual pixel. The line valid signal synchronizes each row or line. The frame valid sig- nal synchronizes each frame.

Figure 13: Timing Diagram for FINCH’s Par- allel Output Camera

The STM32 family of microcontrollers by STMi- croelectronics (ST) was primarily selected due to its dedicated peripheral for parallel camera data, the Digital Camera Interface (DCMI). It was also se- lected because of its widespread adoption, as well as a large online community with many open-source designs that can be referenced.

The DCMI peripheral must be used in conjunc- tion with the direct memory access (DMA) sys- tem.47 DMA is a method of transferring data from one location in the microcontroller to another with- out the CPU. The application note for DCMI47

notes that “DMA2 ensures the transfer from the DCMI to the memory (internal SRAM or external

Miles 11 36th Annual Small Satellite Conference

SRAM/SDRAM) for all STM32 devices embedding the DCMI”. For reasons described below, using RAM to hold camera data does not meet scientific requirements, so a new flow is proposed.

Based on scientific requirements, the payload would ideally take a 60 FPS sequence of frames at 512 × 640 resolution with a bit depth of 14 bits for approximately 10 s while the satellite passes over the ground target. This produces an upper bound of 368 MB per imaging pass. Should fewer than 512 rows of pixels be needed for capturing the spectral dimen- sion, cropping will be done onboard. This brings about an issue of inadequate internal SRAM for data from a single imaging pass. An external SRAM or SDRAM memory that is not a ball grid array (BGA) package was unable to be sourced to accommodate the FINCH Eye’s data size, as the maximum capac- ity available was 128 MB.48 A non-BGA package is a payload requirement in order to facilitate manual soldering. The idea of using multiple external RAM modules was entertained, although the payload mi- crocontroller only has capacity to address two exter- nal SDRAM devices with the flexible memory con- troller. This would give a total capacity of 256 MB, which is not enough for a 368 MB imaging pass.

Figure 14: Image Data Flow through the Mi- crocontroller

The proposed architecture is to stream DCMI via DMA to the Secure Digital and MultiMediaCard (SDMMC) controller which connects to an external SD card. This flow is not explicitly stated to be supported in ST’s documentation. Many reference designs49 stream data to RAM, and only use an SD card for single frame snapshots rather than stream-

ing multiple frames directly to an SD card. Test- ing with STM32 Nucleo development boards and SD card breakout boards will be performed before com- mitting to this architecture. If needed, a custom PCB will be created to achieve better signal integrity compared to using breakout boards.

If this proposed architecture can stream camera data to an SD card without dropped frames, it would have two additional benefits. The NAND flash mem- ory in SD cards is non-volatile, and SD cards with gigabytes of capacity are readily available. Both of these are improvements over the SDRAM solution, which is volatile and has lower capacity. If the pro- posed architecture does not work, the bitrate would need to be decreased by reducing the FPS or image resolution.

Figure 14 shows the image data flow through the microcontroller. The Advanced High-Performance Bus (AHB) matrix is visualized as an abstract cloud because firmware work in that area is ongoing and we do not yet have complete clarity into its opera- tion.

Onboard Image Compression

The radio frequency (RF) downlink is antici- pated to be the bottleneck in FINCH’s data chain. As such, lossless compression of the acquired hy- perspectral data is to be performed onboard the satellite prior to its downlinking to the ground sta- tion, in order to reduce the RF bandwidth re- quired. The compression algorithm design follows the CCSDS123 standard for low-complexity lossless and near-lossless multispectral and hyperspectral data compression,50 which meets FINCH’s require- ments of lossless hyperspectral compression. This standard is backed by a large consortium of space agencies such as NASA, ESA, and JAXA. There exist numerous open-source implementations in C, Java, and for FPGAs as well.

A working implementation in Python can be found on the Image Compression Algorithms GitHub, which achieves lossless compression ratios of ∼2 on a ∼50 MB dataset. Python was selected for initial prototyping to facilitate in-depth under- standing as well as verification. Translation to the C language was then undertaken. Native ARM float- ing point operations, available via the Digital Sig- nal Processor (DSP) core,51 are used to accelerate floating point and vector math operations in the algorithm. Although virtually all academic papers published that discuss the performance of this stan- dard have implemented their designs on FPGAs, the complexity of such a design would require signifi-

Miles 12 36th Annual Small Satellite Conference

cant time spent building expertise, rendering it an unfavourable choice for the team. Pivoting to an FPGA-based design would be considered should the optimised C design take longer than the duration of five orbits (∼450 min) to compress data from one imaging pass. This time requirement was guided by the predicted average downtime between imag- ing passes from operations scheduling.

PAYLOAD OPERATIONS AND MANOEU- VRES

The FINCH optical payload employs a pushb- roommechanism, chosen for its straightforward opti- cal design and spaceflight heritage. During imaging, each individual frame captured by the detector array contains a spatial and a spectral dimension, with the spatial dimension corresponding to a single line of ground pixels oriented in the across-track direction. The along-track spatial dimension is captured by the orbital motion of the spacecraft. The ADCS aboard FINCH actively engages during imaging passes to coordinate the pointing of the entire spacecraft with the frame rate of the sensor core such that a hy- perspectral data cube of sufficient quality can be acquired. Forward motion compensation (FMC) is required to slew the satellite backwards in the pitch direction because the sensor’s frame rate is unable to match the speed of the orbiting spacecraft relative to the ground target. By performing FMC, the satel- lite is able to scan the image target region without any gaps. Figure 15 shows a visual representation of the manoeuvres required for imaging passes.

FINCH is nominally a nadir-imaging instrument; however, imaging can be done at off-nadir angles through ADCS slewing to the extent at which the ground resolution remains reasonably uncompro- mised. A larger range of off-nadir imaging allows for an increased data temporal resolution, referring to the frequency of valid imaging opportunities that FINCH will have. When restricted to nadir imag- ing, the chosen sun-synchronous orbit offers a 15- day revisit time. Thus, a trade-off is to be made. A maximum off-nadir angle of 30 degrees corresponds to 5-day clusters of daily imaging windows (over the site of interest) separated by 10-day periods of down- time, in which tasks such as onboard processing, downlinking, and on-orbit calibration may be sched- uled. This allows for study of daily fluctuations as well as fortnightly trends in data.

Due to the radiation, thermal, and vacuum en- vironmental conditions in low earth orbit, drift in sensor parameters is expected over the course of FINCH’s mission lifetime. As such, on-orbit calibra-

tion is intended to be performed between imaging passes at least three times during the mission life- time. On-orbit calibration can typically be achieved by imaging a location with high spatial uniformity, spectral stability, and time invariance, known as a pseudo-invariant calibration site. The Niger 1 test site from the USGS Test Sites Catalog52 was selected as FINCH’s calibration site due to its high unifor- mity and FINCH’s frequent passes over the region.53

When an image is taken, the known radiance levels can be used to update sensor parameters such as its flat-field characterization. The information obtained from on-orbit calibration can be enhanced using a side slither manoeuvre,54 in which the spacecraft is yawed by 90 degrees such that each detector cap- tures the same scene with the same illumination, ef- fectively producing a flat field input. The spacecraft performs imaging as shown in Figure 15, from this yawed angle. This manoeuvre can improve calibra- tion accuracy by 1–2%, but is still being investigated for feasibility.54

Figure 15: Image Capture Process for Scien- tific and Calibration Images

DATA PROCESSING

Raw data from the instrument is affected by geometric and radiometric errors which must be corrected in order to effectively analyze the data. A ground processing pipeline was established for FINCH, guided by NASA’s and Sentinel-2’s docu- mentation of data processing levels.55,56

Data Processing Levels

The pipeline is described in terms of data pro- cessing levels, spanning Levels 0 through 2. Table 5 below describes the data produced at each level.

Miles 13 36th Annual Small Satellite Conference

Table 5: Data Obtained at each Data Pro- cessing Level

Level Data Product Description

0 Decompressed, communications error-corrected

1A Time-referenced; appended with telemetry, radiometric†, and geometric parameters

1B Radiometrically* and geometrically** corrected 2 Atmospheric processing and retrieval

† from on-orbit calibration * dark noise correction, bad pixel correction, flat field cor- rection, and destriping

- * smile and keystone correction, orthorectification, coreg- istration, and georeferencing

FINCH aims to provide open-source Level 1B data, which can be used by the public for atmo- spheric analysis. The focus thus lies in correcting ra- diometric errors, caused by inconsistencies between individual detectors of the CMOS sensor, as well as geometric errors, caused by optical artifacts. Foot- notes below Table 5 show the corrections performed by FINCH. The FINCH data processing team is cur- rently implementing adapted smile correction and destriping algorithms.

Smile Distortion Correction

Smile distortion involves the mis-mapping of spectral bands to other columns in the spectral di- mension of a hyperspectral image.57 This is caused by optical aberrations and misalignments due to pushbroom systems recording across-track and spec- tral pixels at the same time.58 Smile distortions are to be corrected following the process described by Md. Aktarazzaman: the spectral shift is first quan- tified using a comparison process, and later corrected through cubic spline interpolation.59 By comparing the test spectra to reference spectra, the spectral shift from a smile distortion can be obtained.

Destriping

Striping is a common radiometric error seen in most remote sensing images, appearing as stripes or streaks across the image.60 Different types of striping can occur, including true striping, caused by incorrect relative gain; oblique stripes, slanted stripes caused by geometric registration; and satura- tion striping, only visible over bright and saturated targets. Commonly used destriping algorithms are constructed for specific sensors or data types, requir- ing in-depth knowledge of sensor model and imaging parameters, and may require human judgement for more complex stripes.60 FINCH opted for a neu- ral network-based algorithm, bypassing the need for

comprehensive knowledge of sensor and imaging pa- rameters, due to the generalizable nature of the ap- proach. Following the SURE algorithm presented by Han V. Nguyen et al. (2020),61 static noise was suc- cessfully removed from bands 57, 27, and 17 of the Pavia University dataset,62 a hyperspectral dataset collected over the city of Pavia, Italy, using the re- flective optics system imaging spectrometer (ROSIS- 3). As shown in Figure 17, the performance of the model is evaluated by the peak signal to noise ratio (PSNR) and the mean squared error (MSE) between the original image and the denoised image. Both of these metrics represent the quality of the reconstruc- tion of the image through denoising. A lower MSE refers to fewer discrepancies between images, and a higher PSNR refers to a higher quality image due to the greater difference between the signal (the origi- nal image) and the added noise. As training itera- tions increase, the training loss decreases while the PSNR increases, signifying that the denoised image becomes more similar to the original image.

Figure 17: Destriping Algorithm Perfor- mance on Noisy Data

LINEAR ERROR ANALYSIS

Tool Implementation

LEA is a tool used to mathematically relate pay- load performance to the scientific usefulness of the intended mission. It does so by producing a math- ematical model63 of the payload that encodes SNR performance and systematic errors, producing an es- timate of a known atmospheric state.64 LEA also includes a model of the atmosphere to provide a ref- erence for assessing how well different molecules will be detected by the FINCH Eye payload. Further de- tails on specific equations used in the algorithm and the input values can be found on the Linear Error Analysis GitHub.

Miles 14 36th Annual Small Satellite Conference

By evaluating how well a certain payload com- position is able to estimate the atmospheric state, referred to as the percent error, design tradeoffs and optimizations can be made at a high level. As a student team, there are numerous restrictions, in- cluding budget, time commitment, and expertise. By targeting the critical design drivers that affect the scientific usefulness of the mission, the payload can achieve acceptable performance under the es- tablished constraints. This tool can also be used to assess the overall feasibility of a proposed mission profile.

Key Performance Insights

Hyperspectral cameras can benefit from high spectral resolution, making them useful for atmo- spheric sensing applications. For imaging methane, it is recommended to use a camera with a spectral resolution of at least 0.2 nm.65 Figure 16a shows the relationship between spectral resolution and per- cent error for the FINCH Eye. The percent er- ror is the error between the estimated measurement from the FINCH Eye model produced in LEA and the atmospheric state consisting of concentrations of methane, carbon dioxide, and water vapour.

Counterintuitively, spectral resolution has an in- verse effect on the percent error, with the error de- creasing as spectral resolution becomes worse. This is due to the close dependence of SNR on spec- tral resolution. As the spectral resolution improves, there is less light, or signal, reaching each band that the camera is detecting, thus decreasing the SNR. This decrease in SNR causes an increase in percent error. This highlights SNR as a principal design driver for the FINCH Eye design, when targeting an atmospheric sensing mission. Based on this anal- ysis, optical components and positioning should pri-

oritize SNR above other performance metrics to best achieve atmospheric remote sensing performance re- quirements.

Figure 16b shows the relationship between sig- nal to noise ratio (SNR) and the percent error. SNR clearly has a large effect on minimizing the percent error. Assuming a 25% percent error is acceptable for the needs of the mission, and given the con- straints of the team, a SNR of at least 2000 would be required for imaging methane successfully. This was deemed infeasible based on all FINCH Eye sim- ulations, requiring a 100× increase in performance to achieve. This quantitatively describes what moti- vated the pivot from a methane remote sensing mis- sion to a crop residue mapping mission.

MISSION PROFILE: CROP RESIDUE MAPPING

In this updated mission profile, the scientific imaging site would be an agricultural study site where crop residue retention is being practised on certain fields. From each hyperspectral image, crop residue and soil endmembers would then be ex- tracted from selected pixels as inputs to an SMA algorithm. The resulting percent values of crop residue coverage derived from SMA would then be validated against ground truth measurements taken of the same site, using a statistical analysis metric such as root mean square error (RMSE). The quan- tification of this error between satellite and ground truth measurements would inform the accuracy of the crop residue mapping data. In doing so, FINCH would be contributing a valuable proof of concept for the continued development of crop residue mapping methods via hyperspectral remote sensing.

Many of the spectral index-based methods used by remote sensing missions to quantify crop residue

(a) Estimated Error as a Function of Spectral Res- olution for Methane, Carbon Dioxide, and Water Vapour

(b) Estimated Error as a Function of SNR at a Spectral Resolution of 2.0 nm for Methane, Car- bon Dioxide, And Water Vapour

Miles 15 36th Annual Small Satellite Conference

cover generally require a high SNR and spectral res- olution, along with a specific spectral range for ac- curate results.66 This is due to their dependence on specific fine absorption features associated with crop residue, similar to the mechanism behind at- mospheric sensing.

Since SMA relies only on the self-contained end- member spectra unique to each image, the required SNR and spectral resolution are consequently much lower. When applied to hyperspectral data, SMA al- gorithms have been shown to return acceptably low RMSE values at an SNR of 30,67 which is far more feasible than the SNR of 2000 required for CH4 re- trieval.

Additionally, since SMA requires only that the number of spectral bands be one greater than the number of endmembers used,68 a spectral resolution as coarse as 10 nm is acceptable for hyperspectral sensors. Again, this greatly alleviates the strict re- quirement of a spectral resolution better than 1 nm, which was previously required for atmospheric sens- ing of CH4.

Although there is ostensibly no specific required spectral range for SMA to work, its application to crop residue mapping in multispectral studies has been found most effective when near-infrared (NIR) and SWIR bands are included.2 With this in mind, the spectral range of FINCH would ideally be ex- tended to include the full possible sensor range of 900-1700 nm in order to yield measurements compa- rable to literature.

In order for accurate identification of endmem- ber pixels to occur, spatial resolution for crop residue mapping must be finer than the smallest anticipated unit of crop residue coverage. This exact value is de- pendent on the size of fields in which crop residue retention is being practised, which can vary between agricultural sites. Accordingly, the required swath is also flexible depending on the specific area of in- terest. Given the largest field dimensions currently accessible for measurements in Canada,2 an esti- mated swath of 10-20 km and spatial resolution ap- proaching 30 m is recommended, though not strictly required. While this is a stricter recommendation than the 100 m spatial resolution previously required for atmospheric sensing of landfills, the overall re- quirements for scientifically useful results from crop residue mapping via SMA are much more likely to be feasible for the FINCH Eye to achieve. Table 6 summarises the comparison of scientific re- quirements between the methane monitoring and crop residue mapping mission profiles.

Table 6: Key Requirements for the Methane Monitoring and Crop Residue Mapping Mis- sions

Parameter Methane Mission

Requirement

Crop Residue Mapping

Requirement

Spectral Range 1600–1680 nm 900–1700 nm

Spectral Resolution < 1 nm < 10 nm

Spatial Resolution 100 m 30 m

Swath 50 km 10-20 km

Signal-to-noise ratio 2000 30

Mission Lifetime 1 year 1 year

FUTURE WORK

Due to the updated mission profile, the FINCH Eye will be redesigned to encompass the new sci- entific requirements. In particular, this will con- sider the spectral and spatial resolution as it affects the optical assembly, payload spacing, and data size. Since the new spectral range aligns with that of the sensor, investigation into the detection limit drop- off at either end (900 nm and 1700 nm) as a func- tion of spatial position will be performed to deter- mine whether cost and Z-axis volume consumption can be saved by eliminating the primary bandpass filter from the FINCH Eye. Additionally, spectral wavelengths near the limits of the FLIR Tau’s spec- tral range have a lower quantum efficiency, meaning SNR will decrease. To ensure that the camera’s out- put data is scientifically relevant, an SNR analysis will be performed to quantify the FINCH Eye’s per- formance.

Based on the current model for spatial resolu- tion, shown in Figure 8, meeting the 30 m require- ment necessary for crop residue mapping would cor- respond to a focal length around 300 mm, which exceeds the FINCH Eye’s volume constraints. This requirement-design relationship will be further ex- plored following the process detailed in Figure 1 through further consultation with researchers and imaging sites, as well as optical optimization. Fi- nally, a finer spatial resolution would increase the size of FINCH’s hyperspectral data in two dimen- sions, which would further strain downlink require- ments. However, a reduced spectral resolution is ac- ceptable with the SMA. Further analysis will allow us to quantify the spatial-spectral resolution trade- off necessary to meet data size requirements.

Ongoing coordination with Agriculture and Agri- Foods Canada (AAFC) research teams is taking place to determine which locations will be avail- able for ground truth measurements at the time of

Miles 16 36th Annual Small Satellite Conference

FINCH’s launch. In the meantime, there is more work to be done on selecting the specific SMA algo- rithm that will be used.

For on-orbit calibration, continued investigation into ADCS capabilities will allow us to gauge the ac- curacy of flat-field correction through the feasibility of performing a side slither maneuver.

To validate FINCH’s current optomechanical de- sign, launch vibration conditions and loads will be simulated using finite element analysis with Simcen- ter 3D. In particular, detailed design surrounding the mounting design will be crucial in the vibration isolation of the FLIR Tau sensor.

For thermal design, the diffracting mechanism around the grism is highly sensitive to temperature variations. To validate optomechanical and ther- mal supports and to determine the necessity for an additional active heater/cooler within the payload, Structural, Thermal, Optical Performance (STOP) analysis will be performed. STOP analysis will inte- grate the finite element models that the Structures and Thermal teams are preparing. Iteration through the STOP analysis pipeline will drive detailed design decisions to the payload.

Following the finalization of FINCH’s engineer- ing model, the vibration campaign will begin in Q1– Q2 2023. TVAC testing is planned for Q1 2024, with FINCH currently aiming for a Q3–Q4 2024 launch.

Acknowledgements

UTAT would like to acknowledge Synopsys for their guidance and generosity in providing CODE V optical simulation software and technical support. UTAT would also like to acknowledge Altium, Das- sault Systèmes, and Siemens for their generosity in providing Altium, Solidworks, and NX software and accompanying technical support. Digikey has also discounted numerous products used for payload de- sign development.

UTAT would also like to acknowledge the fol- lowing experts for their guidance: Professor Aaron Berg, Alexander Axiotis, Professor Arthur Chan, Brent Brakeboer, Professor Cameron Proctor, Chris Robson, Professor Christopher Gore, Conor Ander- son, Professor Danijela Puric-Mladenovic, Profes- sor David Risk, Professor Debra Wunch, Dr. Felix Vogel, Dr. Heather McNairn, James Slifierz, Pro- fessor Jennifer Murphy, Dr. Jochen Landgraf, Dr. John Saunders, Dr. Jonas Simon Wilzewski, Pro- fessor Kaley Walker, Professor Li Qian, Dr. Liang- hai Wu, Professor Marianne Hatzopoulou, Najmus Ibrahim, Dr. Namrata Shrestha, Patrick Fancott, Dr. Phuong Dao, Dr. Ray Nassar, Sarah McKenzie- Picot, Dr. Shaojie Chen, Professor Suresh Sivanan-

dam, Dr. Thomas Fox, Tymen Nagel, Wes Funk, Professor William Gough, and Professor Yuhong He.

The FINCH team is fondly appreciative of sev- eral UTAT alumni for their continued support and guidance, including Dylan Vogel, Eric van Velzen, Jaden Reimer, and Lorna Lan.

Lastly, UTAT would like to thank the University of Toronto, including the student body who provide a continuous source of funding, and the University of Toronto Entrepreneurship program for providing UTAT with lab space to make FINCH a reality.

Resources

A few repositories used for analysis in this work are available at the spacesys-finch GitHub, as mentioned in the text. The Payload

Designer, Image Compression Algorithms, and Linear Error Analysis repositories can all be ac- cessed through the hyperlinks.

References

[1] Christian Frankenberg, U Platt, and T Wag- ner. Iterative maximum a posteriori (IMAP)- DOAS for retrieval of strongly absorbing trace gases: Model studies for CH4 and CO2 retrieval from near infrared spectra of SCIAMACHY on- board ENVISAT. Atmospheric Chemistry and Physics, 5(1):9–22, 2005.

[2] Anna Pacheco and Heather McNairn. Evaluat- ing multispectral remote sensing and spectral unmixing analysis for crop residue mapping. Remote Sensing of Environment, 114(10):2219– 2228, 2010.

[3] Thomas R Loveland and John L Dwyer. Land- sat: Building a strong future. Remote Sensing of Environment, 122:22–29, 2012.

[4] Lars Alminde, Morten Bisgaard, Dennis Vinther, Tor Viscor, and Kasper Ostergard. Ed- ucational value and lessons learned from the AAU-CubeSat project. In International Con- ference on Recent Advances in Space Technolo- gies, 2003. RAST’03. Proceedings of, pages 57– 62. IEEE, 2003.

[5] Akito Enokuchi, Masaki Nagai, Ryu Funase, Yuya Nakamura, and Shinichi Nakasuka. Re- mote sensing by University of Tokyo’s pico- satellite project “PRISM”. In Small Satellites for Earth Observation: Selected Proceedings of the 5th International Symposium of the Interna- tional Academy of Astronautics, Berlin, April 4–8 2005, page 169. Walter de Gruyter, 2011.

Miles 17 36th Annual Small Satellite Conference

[6] Karan Sarda, Stuart Eagleson, Eric Caillibot, Cordell Grant, Daniel Kekez, Freddy Prana- jaya, and Robert E Zee. Canadian advanced nanospace experiment 2: Scientific and techno- logical innovation on a three-kilogram satellite. Acta Astronautica, 59(1-5):236–245, 2006.

[7] Tina Hilbig, Klaus Bramstedt, Mark We- ber, John P Burrows, and Matthijs Krijger. Optimised degradation correction for SCIA- MACHY satellite solar measurements from 330 to 1600 nm by using the internal white light source. Atmospheric Measurement Techniques, 13(7):3893–3907, 2020.

[8] Claudio Galeazzi, Andrea Sacchetti, Andrea Cisbani, and Gianni Babini. The PRISMA pro- gram. In IGARSS 2008-2008 IEEE Interna- tional Geoscience and Remote Sensing Sympo- sium, volume 4, pages IV–105. IEEE, 2008.

[9] Akihiko Kuze, Hiroshi Suto, Masakatsu Naka- jima, and Takashi Hamazaki. Thermal and near infrared sensor for carbon observation Fourier- transform spectrometer on the greenhouse gases observing satellite for greenhouse gases moni- toring. Applied optics, 48(35):6716–6733, 2009.

[10] HySIS (Hyperspectral Imaging Satellite). https://directory.eoportal.org/web/

eoportal/satellite-missions/content/-

/article/hysis.

[11] Planet imagery and archive. https://www.

planet.com/products/planet-imagery/, Sep 2021.

[12] Dylan Jervis, Jason McKeever, Berke OA Du- rak, James J Sloan, David Gains, Daniel J Varon, Antoine Ramier, Mathias Strupler, and Ewan Tarrant. The GHGSat-D imaging spec- trometer. Atmospheric Measurement Tech- niques, 14(3):2127–2140, 2021.

[13] Abdul-Halim Jallad, Zulkifli Aziz, Aisha Al- lam, Prashanth Marpu, Alexandros Tsoupos, and Abdulla Marar. MeznSat: A CubeSat for greenhouse gases monitoring and algal blooms prediction. 2018.

[14] U R Rao Satellite Centre (URSC). https://www.ursc.gov.in/student-

satellites/html/sathyabamasat.jsp.

[15] Luis Guanter, Hermann Kaufmann, Karl Segl, Saskia Foerster, Christian Rogass, Sabine Chabrillat, Theres Kuester, André Hollstein, Godela Rossner, Christian Chlebek, et al. The EnMAP spaceborne imaging spectroscopy mis- sion for earth observation. Remote Sensing, 7(7):8830–8857, 2015.

[16] Daniel H Cusworth, Daniel J Jacob, Daniel J Varon, Christopher Chan Miller, Xiong Liu, Kelly Chance, Andrew K Thorpe, Riley M Duren, Charles E Miller, David R Thompson, et al. Potential of next-generation imaging spec- trometers to detect and quantify methane point sources from space. Atmospheric Measurement Techniques, 12(10):5655–5668, 2019.

[17] AJ Turner, Daniel J Jacob, Kevin J Wecht, Jo- hannes D Maasakkers, E Lundgren, Arlyn E Andrews, Sebastien C Biraud, Hartmut Boesch, Kevin W Bowman, Nicholas M Deutscher, et al. Estimating global and North Ameri- can methane emissions with high spatial res- olution using GOSAT satellite data. Atmo- spheric Chemistry and Physics, 15(12):7049– 7069, 2015.

[18] H McNairn and R Protz. Mapping corn residue cover on agricultural fields in Oxford County, Ontario, using Thematic Mapper. Cana- dian Journal of Remote Sensing, 19(2):152–159, 1993.

[19] PL Nagler, CST Daughtry, and SN Goward. Plant litter and soil reflectance. Remote Sens- ing of Environment, 71(2):207–215, 2000.

[20] Anna Pacheco, Heather McNairn, Delmar Holmstrom, and Eric Gauthier. Using earth ob- servation to monitor no-till practices over agri- cultural crops in Eastern Ontario and Prince Edward Island, Canada. In CRSS/ASPRS 2007 Specialty Conference, Ottawa, Ontario, Canada, October 28–November 1, 2007.

[21] A Pacheco and H McNairn. Mapping crop residue cover over regional agricultural land- scapes in canada. Agriculture and Agri-Food Canada, 960, 2012.

[23] Randy A Kimble, John W MacKenty, and Jacqueline A Townsend. Wide Field Camera 3: a powerful new imager for the Hubble Space Telescope. In Space Telescopes and Instrumen- tation 2008: Optical, Infrared, and Millimeter, volume 7010, pages 431–442. SPIE, July 2008.

[24] Thomas P Greene, Laurie Chu, Eiichi Egami, Klaus W Hodapp, Douglas M Kelly, Jarron Leisenring, Marcia Rieke, Massimo Robberto, Everett Schlawin, and John Stansberry. Slitless spectroscopy with the James Webb Space Tele- scope Near-Infrared Camera (JWST NIRCam). In Space Telescopes and Instrumentation 2016: Optical, Infrared, and Millimeter Wave, volume 9904, pages 130–141. SPIE, July 2016.

Miles 18 36th Annual Small Satellite Conference

[25] Dominic A Ludovici and Robert L Mutel. A compact grism spectrometer for small opti- cal telescopes. American journal of physics, 85(11):873–879, November 2017.

[26] Timo Hyvärinen, Esko Herrala, Wes Pro- cino, and Oliver Weatherbee. Compact high-resolution VIS/NIR hyperspectral sensor. In Next-Generation Spectroscopic Technologies IV, volume 8032, pages 237–244. SPIE, May 2011.

[27] Zsolt Volent, Geir Johnsen, and Fred Sigernes. Kelp forest mapping by use of airborne hyper- spectral imager. Journal of Applied Remote Sensing, 1(1):011503, December 2007.

[28] Masako Kashiwagi, Keiko Oka, Misako Irisawa, Noboru Ebizuka, Masanori Iye, and Kashiko Kodate. Optimal design and fabrication of high dispersion VPH grism for Subaru Telescope. In Optical Fabrication, Metrology, and Mate- rial Advancements for Telescopes, volume 5494, pages 217–227. SPIE, September 2004.

[29] Nasrin Mostafavi Pak, Sajjan Heerah, Junhua Zhang, Elton Chan, Doug Worthy, Felix Vogel, and Debra Wunch. The facility level and area methane emissions inventory for the greater toronto area (flame-gta). Atmospheric Environ- ment, 252:118319, 2021.

[30] Joannes D Maasakkers, Daniel J Jacob, Melissa P Sulprizio, Tia R Scarpelli, Hannah Nesser, Jianxiong Sheng, Yuzhong Zhang, Xiao Lu, A Anthony Bloom, Kevin W Bowman, et al. 2010–2015 north american methane emis- sions, sectoral contributions, and trends: a high-resolution inversion of gosat observations of atmospheric methane. Atmospheric Chem- istry and Physics, 21(6):4339–4356, 2021.

[31] Genevieve Plant, Eric A Kort, Lee T Murray, Joannes D Maasakkers, and Ilse Aben. Evalu- ating urban methane emissions from space us- ing tropomi methane and carbon monoxide ob- servations. Remote Sensing of Environment, 268:112756, 2022.

[32] Environment Canada. National inventory re- port, 1990–2004—greenhouse gas sources and sinks in canada, 2006.

[33] Anne Olhoff, John M Christensen, et al. Emis- sions gap report 2018. UNEP DTU Partner- ship: Copenhagen, Denmark, 2018.

[34] Sebastien Ars, Felix Vogel, Colin Arrow- smith, Sajjan Heerah, Emily Knuckey, Juliette Lavoie, Christopher Lee, Nasrin Mostafavi Pak, Jaden L Phillips, and Debra Wunch. Investi- gation of the spatial distribution of methane

sources in the Greater Toronto Area using mobile gas monitoring systems. Environmen- tal Science & Technology, 54(24):15671–15679, 2020.

[35] Cristina Iacoboaea and Florian Petrescu. Land- fill monitoring using remote sensing: a case study of Glina, Romania. Waste Management & Research, 31(10):1075–1080, 2013.

[36] JP Veefkind, I Aben, K McMullan, H Förster, J De Vries, G Otter, J Claas, HJ Eskes, JF De Haan, Q Kleipool, et al. TROPOMI on the ESA Sentinel-5 Precursor: A GMES mis- sion for global observations of the atmospheric composition for climate, air quality and ozone layer applications. Remote sensing of environ- ment, 120:70–83, 2012.

[37] Sarah Rogers, Jaime Sanchez de la Vega, Yegor Zenkov, Craig Knoblauch, Devon Bautista, Trevor Bautista, Ryan Fagan, Cody Rober- son, Stephen Flores, Raymond Barakat, et al. Phoenix: A CubeSat mission to study the im- pact of urban heat islands within the US. 2020.

[38] CubeSat Design Specification Rev. The Cube- Sat program. Cal Poly SLO, 13, 2017.

[39] Brent Nicholas Anders Brakeboer. Development of the structural and thermal control subsystems for an Earth observation microsatellite and its payload. University of Toronto (Canada), 2015.

[40] Constantine Lukashin, Trevor Jackson, Michael Cooney, Noah Ryan, Joshua Beverly, Cindy Young, Gugu Rutherford, Warren Davis, Thuan Nguyen, Randy Swanson, et al. ARC- STONE: Calibration of lunar spectral re- flectance. 2018.

[41] Y Luo, X Wu, K Wang, and Y Wang. Compar- ative study on surface influence to outgassing performance of aluminum alloy. Applied Sur- face Science, 502:144166, 2020.

[42] Hubs on-demand manufacturing. https://

www.hubs.com/manufacture/.

[43] General environmental verification standard (gevs) for gsfc flight programs and projects.

[44] Jake Cheng, Jakob Lifshits, Cordell Grant, Mi- hail Barbu, and Robert Zee. The BRITE Con- stellation space telescope design and test of a wide field, high resolution, low noise optical telescope for a nanosatellite constellation. 2011.

[45] Jim Burge. Mounting of optical components. SPIE Short Course, 1019, 2011.

[46] Matthew Smith, Amanda Donner, Mary Knapp, Christopher Pong, Colin Smith, Jason Luu, Peter Di Pasquale, and Brian Campuzano.

Miles 19 36th Annual Small Satellite Conference

On-orbit results and lessons learned from the ASTERIA space telescope mission. 2018.

[47] AN5020 application note. https://www.

st.com/resource/en/application_note/

an5020-digital-camera-interface-dcmi-

on-stm32-mcus-stmicroelectronics.pdf. STMicroelectronics.

[48] Memory. https://www.digikey.ca/en/

products/filter/memory/774. Digikey.

[49] UM1549 user manual. https://www.

st.com/resource/en/user_manual/

um1549-stm32-demonstration-builder-

stmicroelectronics.pdf. STMicroelectron- ics.

[50] Low-complexity lossless and near-lossless multispectral and hyperspectral image com- pression. https://public.ccsds.org/Pubs/

123x0b2c3.pdf.

[51] CMSIS DSP Software Library. https:

//www.keil.com/pack/doc/CMSIS/DSP/html/

index.html.

[52] Niger 1. https://calval.cr.usgs.gov/apps/ niger-1.

[53] Aaron Gerace, John Schott, Michael Gart- ley, and Matthew Montanaro. An analysis of the side slither on-orbit calibration technique using the DIRSIG model. Remote Sensing, 6(11):10523–10545, 2014.

[54] Bradley G Henderson and Keith S Krause. Rel- ative radiometric correction of QuickBird im- agery using the side-slither technique on orbit. In Earth Observing Systems IX, volume 5542, pages 426–436. SPIE, 2004.

[55] NASA Earth Science Data Systems. Data pro- cessing levels. https://www.earthdata.nasa. gov/engage/open-data-services-and-

software/data-information-policy/data-

levels.

[56] ESA Sentinel Online. Level-1. https:

//sentinel.esa.int/web/sentinel/user-

guides/sentinel-2-msi/processing-

levels/level-1.

[57] Yuheng Chen, Yiqun Ji, Jiankang Zhou, Xin- hua Chen, XiaoXiao Wei, and Weimin Shen. Distortion measurement of push-broom imag- ing spectrometer. In 2009 International Con- ference on Optical Instruments and Technology: Optical Systems and Modern Optoelectronic In- struments, volume 7506, pages 606–614. SPIE, 2009.

[58] Xavier Ceamanos and Sylvain Douté. Spectral smile correction of CRISM/MRO hyperspectral

images. IEEE Transactions on Geoscience and Remote Sensing, 48(11):3951–3959, 2010.

[59] Md Aktaruzzaman. Simulation and correction of spectral smile effect and its influence on hy- perspectral mapping. ITC, 2008.

[60] Fuan Tsai and Walter W Chen. Striping noise detection and correction of remote sensing im- ages. IEEE Transactions on Geoscience and Remote Sensing, 46(12):4122–4131, 2008.

[61] Han V Nguyen, Magnus O Ulfarsson, and Jo- hannes R Sveinsson. Hyperspectral image de- noising using SURE-based unsupervised convo- lutional neural networks. IEEE Transactions on Geoscience and Remote Sensing, 59(4):3369– 3382, 2020.

[62] Pavia University dataset. https:

//paperswithcode.com/dataset/pavia-

university, 2021.

[63] R G Grainger. An Atmospheric Radiative Transfer Primer, chapter 8—Introduction to Retrieval Theory, page 123–151.

[64] Stephanie P Rusli, Otto Hasekamp, Guangliang Fu, Yasjka Meijer, Jochen Landgraf, et al. An- thropogenic CO2 monitoring satellite mission: the need for multi-angle polarimetric observa- tions. Atmospheric Measurement Techniques, 14(2):1167–1190, 2021.

[65] Prabhunath Prasad, Shantanu Rastogi, and Raghavendra P Singh. Radiative transfer mod- eling of atmospheric methane for satellite mea- surements in the 1.66 micron spectral win- dow. Journal of Near Infrared Spectroscopy, 26(3):196–204, 2018.

[66] Wells Dean Hively, Brian T Lamb, Craig ST Daughtry, Guy Serbin, Philip Dennison, Ray- mond F Kokaly, Zhuoting Wu, and Jeffery G Masek. Evaluation of SWIR crop residue bands for the Landsat next mission. Remote Sensing, 13(18):3718, 2021.

[67] Yang Shao, Jinhui Lan, Yuzhen Zhang, and Jin- lin Zou. Spectral unmixing of hyperspectral re- mote sensing imagery via preserving the intrin- sic structure invariant. Sensors, 18(10):3528, 2018.

[68] John B Adams, Donald E Sabol, Valerie Ka- pos, Raimundo Almeida Filho, Dar A Roberts, Milton O Smith, and Alan R Gillespie. Classi- fication of multispectral images based on frac- tions of endmembers: Application to land-cover change in the Brazilian Amazon. Remote sens- ing of Environment, 52(2):137–154, 1995.

Miles 20 36th Annual Small Satellite Conference