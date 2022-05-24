<script setup>
import {ref, computed} from 'vue'

const props = defineProps({
  showAll: Boolean
})

const papers = ref([{
  "projects": [{
    "operators": ["5d24ef150a41d55c7402e029", "5d24e56b8dd3ea3f3408283d"],
    "contributors": [],
    "developers": ["5d24ba8a1c7476627c24f453", "5d82891fd0ceb47de1329ba6"],
    "leadership": ["5d24e56b8dd3ea3f3408283d"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d63ebff660730666363bf5b",
    "name": "ImageX",
    "url": "https://imagex.sca.iu.edu",
    "description": "ImageX is a set of javascript libraries used to generate and display large-scale scientific images within a web browser.  It utilizes the OpenSeaDragon open-source viewing library, and is currently deployed as part of the ODI-PPA project.",
    "date_created": "2017-10-15T00:00:00.000Z",
    "repo": "https://github.com/IUSCA/imagex",
    "logo": "5db1fd9eea2de06d5ef82053",
    "screenshots": [{
      "_id": "5d63ebff660730666363bf5f",
      "caption": "ImageX RGB colorization example",
      "image": "5d63ebff660730666363bf46"
    }, {
      "_id": "5d63ebff660730666363bf5e",
      "caption": "ImageX image details page",
      "image": "5d63ebff660730666363bf47"
    }, {
      "_id": "5d63ebff660730666363bf5d",
      "caption": "ImageX Dark Energy Camera demo",
      "image": "5d63ebff660730666363bf52"
    }],
    "__v": 6,
    "view_rank": 25,
    "short_url": "imagex"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }, {
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }, {
    "active": true,
    "_id": "5d24ef150a41d55c7402e029",
    "role": "Operations Lead",
    "name": "Raymond Perigo",
    "email": "rperigo@iu.edu",
    "headshot": "6244731c0f3fcc2f7573ec35",
    "__v": 0,
    "background": "RHCE Certification",
    "joined": "2016-07-01T00:00:00.000Z",
    "sca": true,
    "uid": "rperigo",
    "view_rank": 3
  }],
  "_id": "5d70098e79e7371d5c3bab84",
  "bib_string": "Young, M. D., Gopu, A., Perigo, R. 2018. ImageX 3.0: A Full Stack Imaging Archive Solution. Proc. SPIE 10707, Software and Cyberinfrastructure for Astronomy V, 107071A (6 July 2018);",
  "date": null,
  "doi": "https://doi.org/10.1117/12.2313684",
  "project": "5d63ebff660730666363bf5b",
  "links": [{
    "_id": "5d70098e79e7371d5c3bab86",
    "url": "https://drive.google.com/file/d/1Prjz8ngeKc0QzyDf9I5oD0v4UDDsNQQU/view?usp=sharing",
    "label": "Online abstract (PDF)"
  }, {
    "_id": "5d70098e79e7371d5c3bab85",
    "url": "https://drive.google.com/file/d/1pozzPuX7YifSCTUqLl_vKFkS4ywXAYPr/view?usp=sharing",
    "label": "Full paper (PDF)"
  }, {
    "_id": "5d711ccc4db0c0676e56cdc6",
    "url": "https://drive.google.com/file/d/1U_zhDUqZQ-CCxMbqqIbampQ0YgaUbNdO/view?usp=sharing",
    "label": "Conference presentation slides (PDF)"
  }],
  "__v": 2
}, {
  "projects": [{
    "operators": ["5d24ef150a41d55c7402e029", "5d24e56b8dd3ea3f3408283d"],
    "contributors": ["5d9cc3e9cb13e070e251395c"],
    "developers": [],
    "leadership": ["5d24e56b8dd3ea3f3408283d"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d76b516389a4b04b4c45100",
    "name": "SCA-OPS",
    "url": "n/a",
    "description": "Backing up our software development and project management services, SCA provides a strong operational background to ensure these services are reliable, performant, and secure. We, under the SCA-OPS (DevOps) umbrella, operate several dozen systems running on our own on-premises physical hardware (both physical and QEMU/KVM virtual machines), as well as IU Intelligent Infrastructure and Google Cloud VMs.\nTo support the user-facing elements of our services, SCA Operations provides a number of backend components and operational tools:\n\n- Nginx \twebservers with load-balancing and reverse proxy setups where needed\n- Centralized MongoDB and MariaDB database servers, as well as a number of \tproject-local database servers where a centralized solution would be \timpractical\n- Message passing services like RabbitMQ\n- A namespaced Squid proxy service for secured systems with local-only \tnetwork access\n- Custom Docker containers to deploy and sandbox custom and legacy code and an Docker container utilization when applicable\n- Centralized syslog-ng for storage of system logfiles\n- ELK for auditing and insight into system access patterns and anomalies\n- Sensu monitoring of real-time server status, including custom network \tchecks for firewall holes from a remote subnet\n- Extensible LVM-based storage on all Linux systems\n- A custom IPTables wrapper with multiple failsafes and reduced configuration overhead\n- Centralized configuration management via Ansible and Puppet, providing a stable base deployment shared among all systems\n\nWe strive to balance security and reliability with ease-of-use. In collaboration with the IU Center for Advanced Cybersecurity Research (CACR), we have developed a comprehensive set of security controls based on NIST-800-53. We support projects that work with electronically Protected Health Information (ePHI), and the bulk of these same controls are in place on all systems we operate",
    "date_created": "2010-06-01T00:00:00.000Z",
    "screenshots": [{
      "_id": "5d81137ea95efe12fcbead65",
      "caption": "Example Grafana plots for one of the SCA servers.",
      "image": "5d81137ea95efe12fcbead63"
    }],
    "__v": 10,
    "view_rank": 3,
    "logo": "5d791af50bb9b57043cb8281",
    "short_url": "ops"
  }, {
    "operators": ["5d24e56b8dd3ea3f3408283d", "5d24ef150a41d55c7402e029", "5d24ba8a1c7476627c24f453"],
    "contributors": ["5d9cc2fbcb13e070e2513953", "5d9cc37ecb13e070e2513959", "5d9cc33bcb13e070e2513956"],
    "developers": ["5d24ba8a1c7476627c24f453", "5d82891fd0ceb47de1329ba6", "5d24ef660a41d55c7402e02c", "5d24e56b8dd3ea3f3408283d"],
    "leadership": ["5d24e56b8dd3ea3f3408283d", "5d828aecd0ceb47de1329ba9", "602af1bd870e9f3010f48713", "602af2c7870e9f3010f4871f", "602af287870e9f3010f4871c"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d262d7018b75a1d0b51f913",
    "name": "ODI-PPA",
    "url": "https://portal.odi.iu.edu",
    "description": "The One Degree Imager (ODI), an optical imager on the WIYN 3.5m telescope at Kitt Peak, Arizona, is designed to deliver \natmosphere-limited image quality (<0.4”) over a one degree field of view. The ODI Pipeline, Portal, and Archive (ODI-PPA) is a web science\ngateway that provides astronomers a single point of access to ODI data, and rich computational and visualization capabilities. Its goal is to\nsupport scientists in handling complex data sets, and to enhance the WIYN observatory's scientific productivity beyond data acquisition.",
    "date_created": "2010-05-03T00:00:00.000Z",
    "repo": "https://github.com/IUSCA/odi-portal/",
    "logo": "5db1fd0eea2de06d5ef8204d",
    "screenshots": [{
      "_id": "5d262d7018b75a1d0b51f917",
      "caption": "ODI-PPA Image Details page showing preview and quality assurance plot",
      "image": "5d262d7018b75a1d0b51f906"
    }, {
      "_id": "5d262d7018b75a1d0b51f916",
      "caption": "ODI-PPA homepage",
      "image": "5d262d7018b75a1d0b51f908"
    }, {
      "_id": "5d262d7018b75a1d0b51f915",
      "caption": "ODI-PPA user dashboard",
      "image": "5d262d7018b75a1d0b51f90a"
    }, {"_id": "5d262d7018b75a1d0b51f914", "caption": "ODI-PPA search page", "image": "5d262d7018b75a1d0b51f90b"}],
    "__v": 12,
    "view_rank": 2,
    "short_url": "odi"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24ef150a41d55c7402e029",
    "role": "Operations Lead",
    "name": "Raymond Perigo",
    "email": "rperigo@iu.edu",
    "headshot": "6244731c0f3fcc2f7573ec35",
    "__v": 0,
    "background": "RHCE Certification",
    "joined": "2016-07-01T00:00:00.000Z",
    "sca": true,
    "uid": "rperigo",
    "view_rank": 3
  }, {
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }, {
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }],
  "_id": "5d711f984db0c0676e56cdc9",
  "bib_string": "Perigo, R., Gopu, A., Young, M. D. 2018. \"Toward sustainable deployment of distributed services on the cloud: dockerized ODI-PPA on Jetstream\", Proc. SPIE 10707, Software and Cyberinfrastructure for Astronomy V, 107072X (6 July 2018); doi:10.1117/12.2313647",
  "date": null,
  "doi": "https://doi.org/10.1117/12.2313647s",
  "project": "5d76b516389a4b04b4c45100",
  "links": [{
    "_id": "5d711f984db0c0676e56cdca",
    "url": "https://drive.google.com/file/d/1mmwJujwFAVO3UarBrkO0r8B27nICrkwe/view?usp=sharing",
    "label": "Online abstract (PDF)"
  }, {
    "_id": "5d80f66da95efe12fcbeacf1",
    "url": "https://drive.google.com/file/d/1I50OkIV9hW4PYH-QI3hXqEW4pPxsI3Zd/view?usp=sharing",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "5d80f66da95efe12fcbeacf0",
    "url": "https://drive.google.com/file/d/19fULyEH9EyXqnkfoTeyBO9dEUHqHU7Oq/view?usp=sharing",
    "label": "Conference Poster (PDF)"
  }],
  "__v": 5
}, {
  "projects": [{
    "operators": ["5d24e56b8dd3ea3f3408283d", "5d24ef150a41d55c7402e029", "5d24ba8a1c7476627c24f453"],
    "contributors": ["5d9cc2fbcb13e070e2513953", "5d9cc37ecb13e070e2513959", "5d9cc33bcb13e070e2513956"],
    "developers": ["5d24ba8a1c7476627c24f453", "5d82891fd0ceb47de1329ba6", "5d24ef660a41d55c7402e02c", "5d24e56b8dd3ea3f3408283d"],
    "leadership": ["5d24e56b8dd3ea3f3408283d", "5d828aecd0ceb47de1329ba9", "602af1bd870e9f3010f48713", "602af2c7870e9f3010f4871f", "602af287870e9f3010f4871c"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d262d7018b75a1d0b51f913",
    "name": "ODI-PPA",
    "url": "https://portal.odi.iu.edu",
    "description": "The One Degree Imager (ODI), an optical imager on the WIYN 3.5m telescope at Kitt Peak, Arizona, is designed to deliver \natmosphere-limited image quality (<0.4”) over a one degree field of view. The ODI Pipeline, Portal, and Archive (ODI-PPA) is a web science\ngateway that provides astronomers a single point of access to ODI data, and rich computational and visualization capabilities. Its goal is to\nsupport scientists in handling complex data sets, and to enhance the WIYN observatory's scientific productivity beyond data acquisition.",
    "date_created": "2010-05-03T00:00:00.000Z",
    "repo": "https://github.com/IUSCA/odi-portal/",
    "logo": "5db1fd0eea2de06d5ef8204d",
    "screenshots": [{
      "_id": "5d262d7018b75a1d0b51f917",
      "caption": "ODI-PPA Image Details page showing preview and quality assurance plot",
      "image": "5d262d7018b75a1d0b51f906"
    }, {
      "_id": "5d262d7018b75a1d0b51f916",
      "caption": "ODI-PPA homepage",
      "image": "5d262d7018b75a1d0b51f908"
    }, {
      "_id": "5d262d7018b75a1d0b51f915",
      "caption": "ODI-PPA user dashboard",
      "image": "5d262d7018b75a1d0b51f90a"
    }, {"_id": "5d262d7018b75a1d0b51f914", "caption": "ODI-PPA search page", "image": "5d262d7018b75a1d0b51f90b"}],
    "__v": 12,
    "view_rank": 2,
    "short_url": "odi"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }],
  "_id": "5d7277a3dec5100b7258575c",
  "bib_string": "Hayashi, S.; Gopu, A.; Young, M. D.; Kotulla, R. 2014. PPA Stack: User Driven Image Stacking for ODI data and beyond via a Highly Customizable Web Interface. Proceedings of The Astronomical Society of the Pacific (ASP) 09/2015, p.421",
  "date": null,
  "doi": "",
  "project": "5d262d7018b75a1d0b51f913",
  "links": [{
    "_id": "5d7277a3dec5100b7258575f",
    "url": "https://ui.adsabs.harvard.edu/abs/2015ASPC..495..421H/abstract",
    "label": "Online Abstract"
  }, {
    "_id": "5d7277a3dec5100b7258575e",
    "url": "https://drive.google.com/file/d/1YIsdEm8iBBW1KY7SOL1pFT3B08BE7Px8/view?usp=sharing",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "5d7277a3dec5100b7258575d",
    "url": "https://drive.google.com/file/d/148EJZcnkXX6N3-iKno4NuQ7RaumMzrRs/view?usp=sharing",
    "label": "Conference Presentation Slides"
  }],
  "__v": 1
}, {
  "projects": [{
    "operators": ["5d24ef150a41d55c7402e029", "5d24e56b8dd3ea3f3408283d"],
    "contributors": [],
    "developers": ["5d24ba8a1c7476627c24f453", "5d82891fd0ceb47de1329ba6"],
    "leadership": ["5d24e56b8dd3ea3f3408283d"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d63ebff660730666363bf5b",
    "name": "ImageX",
    "url": "https://imagex.sca.iu.edu",
    "description": "ImageX is a set of javascript libraries used to generate and display large-scale scientific images within a web browser.  It utilizes the OpenSeaDragon open-source viewing library, and is currently deployed as part of the ODI-PPA project.",
    "date_created": "2017-10-15T00:00:00.000Z",
    "repo": "https://github.com/IUSCA/imagex",
    "logo": "5db1fd9eea2de06d5ef82053",
    "screenshots": [{
      "_id": "5d63ebff660730666363bf5f",
      "caption": "ImageX RGB colorization example",
      "image": "5d63ebff660730666363bf46"
    }, {
      "_id": "5d63ebff660730666363bf5e",
      "caption": "ImageX image details page",
      "image": "5d63ebff660730666363bf47"
    }, {
      "_id": "5d63ebff660730666363bf5d",
      "caption": "ImageX Dark Energy Camera demo",
      "image": "5d63ebff660730666363bf52"
    }],
    "__v": 6,
    "view_rank": 25,
    "short_url": "imagex"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }, {
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }, {
    "active": true,
    "_id": "5d24ef150a41d55c7402e029",
    "role": "Operations Lead",
    "name": "Raymond Perigo",
    "email": "rperigo@iu.edu",
    "headshot": "6244731c0f3fcc2f7573ec35",
    "__v": 0,
    "background": "RHCE Certification",
    "joined": "2016-07-01T00:00:00.000Z",
    "sca": true,
    "uid": "rperigo",
    "view_rank": 3
  }],
  "_id": "5d77eb05389a4b04b4c45103",
  "bib_string": "Young, M. D., Gopu, A., Perigo, R., & Hayashi, S. 2017. Image Archives Made Easy with Docker and ImageX. In ASP Conference Series TBD, Astronomical Data Analysis Software and Systems XXVII.",
  "date": null,
  "doi": "",
  "project": "5d63ebff660730666363bf5b",
  "links": [{
    "_id": "5d77eb05389a4b04b4c45107",
    "url": "https://drive.google.com/file/d/1_9g2_MU3eQu2kumGuly783Ssybfkv2Lu/view?usp=sharing",
    "label": "Online Abstract (PDF)"
  }, {
    "_id": "5d77eb05389a4b04b4c45106",
    "url": "https://drive.google.com/file/d/15XU8jL2r-2ET-lU8QyGULW43ZHDhW8Bu/view?usp=sharing",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "5d77eb05389a4b04b4c45105",
    "url": "https://drive.google.com/file/d/1DmrtrkAwTgysMONuBjGrwHGDvMJ0XtKx/view?usp=sharing",
    "label": "Conference presentation slides (PDF)"
  }, {"_id": "5d77eb05389a4b04b4c45104", "url": "", "label": ""}],
  "__v": 1
}, {
  "projects": [{
    "operators": ["5d24e56b8dd3ea3f3408283d", "5d24ef150a41d55c7402e029"],
    "contributors": [],
    "developers": ["5d24ba8a1c7476627c24f453"],
    "leadership": ["602af287870e9f3010f4871c"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d77ef2a03560c7373554cd3",
    "name": "GCS-SCA",
    "url": "https://gcs.sca.iu.edu/",
    "description": "The Globular Cluster Systems - Scalable Compute Archive ...",
    "date_created": "2016-07-01T00:00:00.000Z",
    "screenshots": [{
      "_id": "5d8112fca95efe12fcbead62",
      "caption": "GCS Search Page",
      "image": "5d8112fca95efe12fcbead60"
    }],
    "__v": 4,
    "view_rank": 19,
    "logo": "5d791bb40bb9b57043cb8285",
    "short_url": "gcs"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }, {
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }],
  "_id": "5d77ef7803560c7373554cd4",
  "bib_string": "Young, M.D.; Rhode, K.L.; Gopu, A. 2015. A Science Portal and Archive for Extragalactic Globular Cluster Systems Data. American Astronomical Society, 225th meeting, Seattle, WA.",
  "date": null,
  "doi": "",
  "project": "5d77ef2a03560c7373554cd3",
  "links": [{
    "_id": "5d77ef7803560c7373554cd6",
    "url": "https://ui.adsabs.harvard.edu/abs/2015AAS...22524723Y",
    "label": "Online abstract "
  }, {
    "_id": "5d77ef7803560c7373554cd5",
    "url": "https://drive.google.com/file/d/128zjf2KJlowLvvs8u_Jw8xQxsbXR-CJe/view?usp=sharing",
    "label": "Conference poster (PDF)"
  }],
  "__v": 1
}, {
  "projects": [{
    "operators": ["5d24ef150a41d55c7402e029", "5d24e56b8dd3ea3f3408283d"],
    "contributors": ["5d9cc3e9cb13e070e251395c"],
    "developers": [],
    "leadership": ["5d24e56b8dd3ea3f3408283d"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d76b516389a4b04b4c45100",
    "name": "SCA-OPS",
    "url": "n/a",
    "description": "Backing up our software development and project management services, SCA provides a strong operational background to ensure these services are reliable, performant, and secure. We, under the SCA-OPS (DevOps) umbrella, operate several dozen systems running on our own on-premises physical hardware (both physical and QEMU/KVM virtual machines), as well as IU Intelligent Infrastructure and Google Cloud VMs.\nTo support the user-facing elements of our services, SCA Operations provides a number of backend components and operational tools:\n\n- Nginx \twebservers with load-balancing and reverse proxy setups where needed\n- Centralized MongoDB and MariaDB database servers, as well as a number of \tproject-local database servers where a centralized solution would be \timpractical\n- Message passing services like RabbitMQ\n- A namespaced Squid proxy service for secured systems with local-only \tnetwork access\n- Custom Docker containers to deploy and sandbox custom and legacy code and an Docker container utilization when applicable\n- Centralized syslog-ng for storage of system logfiles\n- ELK for auditing and insight into system access patterns and anomalies\n- Sensu monitoring of real-time server status, including custom network \tchecks for firewall holes from a remote subnet\n- Extensible LVM-based storage on all Linux systems\n- A custom IPTables wrapper with multiple failsafes and reduced configuration overhead\n- Centralized configuration management via Ansible and Puppet, providing a stable base deployment shared among all systems\n\nWe strive to balance security and reliability with ease-of-use. In collaboration with the IU Center for Advanced Cybersecurity Research (CACR), we have developed a comprehensive set of security controls based on NIST-800-53. We support projects that work with electronically Protected Health Information (ePHI), and the bulk of these same controls are in place on all systems we operate",
    "date_created": "2010-06-01T00:00:00.000Z",
    "screenshots": [{
      "_id": "5d81137ea95efe12fcbead65",
      "caption": "Example Grafana plots for one of the SCA servers.",
      "image": "5d81137ea95efe12fcbead63"
    }],
    "__v": 10,
    "view_rank": 3,
    "logo": "5d791af50bb9b57043cb8281",
    "short_url": "ops"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }, {
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }],
  "_id": "5d80f768a95efe12fcbeacf3",
  "bib_string": "Gopu, A.; Hayashi, S.; Young, M. D.; Kotulla, R.; Henschel, R. 2016. Trident: Scalable Compute Archive, and Visualuzation/Analysiss Systems. Proc. SPIE 9913, Software and Cyberinfrastructure for Astronomy III, 99131H (August 8, 2016); doi:10.1117/12.2233111",
  "date": null,
  "doi": "10.1117/12.2233111",
  "project": "5d76b516389a4b04b4c45100",
  "links": [{
    "_id": "5d80f768a95efe12fcbeacf6",
    "url": "https://www.spiedigitallibrary.org/conference-proceedings-of-spie/9913/1/Trident-scalable-compute-archives-workflows-visualization-and-analysis/10.1117/12.2233111.full",
    "label": "Online Abstract"
  }, {
    "_id": "5d80f768a95efe12fcbeacf5",
    "url": "https://drive.google.com/file/d/1EAyVs9cnKuzD4bKLCOs3qOtfdVEQS_q5/view?usp=sharing",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "5d80f768a95efe12fcbeacf4",
    "url": "https://drive.google.com/file/d/14uGTJNRmAXpRHscViTiMCBCXe1l_Pn1N/view?usp=sharing",
    "label": "Conference presentation slides (PDF)"
  }],
  "__v": 1
}, {
  "projects": [{
    "operators": ["5d24ef150a41d55c7402e029", "5d24e56b8dd3ea3f3408283d"],
    "contributors": ["5d9cc3e9cb13e070e251395c"],
    "developers": [],
    "leadership": ["5d24e56b8dd3ea3f3408283d"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d76b516389a4b04b4c45100",
    "name": "SCA-OPS",
    "url": "n/a",
    "description": "Backing up our software development and project management services, SCA provides a strong operational background to ensure these services are reliable, performant, and secure. We, under the SCA-OPS (DevOps) umbrella, operate several dozen systems running on our own on-premises physical hardware (both physical and QEMU/KVM virtual machines), as well as IU Intelligent Infrastructure and Google Cloud VMs.\nTo support the user-facing elements of our services, SCA Operations provides a number of backend components and operational tools:\n\n- Nginx \twebservers with load-balancing and reverse proxy setups where needed\n- Centralized MongoDB and MariaDB database servers, as well as a number of \tproject-local database servers where a centralized solution would be \timpractical\n- Message passing services like RabbitMQ\n- A namespaced Squid proxy service for secured systems with local-only \tnetwork access\n- Custom Docker containers to deploy and sandbox custom and legacy code and an Docker container utilization when applicable\n- Centralized syslog-ng for storage of system logfiles\n- ELK for auditing and insight into system access patterns and anomalies\n- Sensu monitoring of real-time server status, including custom network \tchecks for firewall holes from a remote subnet\n- Extensible LVM-based storage on all Linux systems\n- A custom IPTables wrapper with multiple failsafes and reduced configuration overhead\n- Centralized configuration management via Ansible and Puppet, providing a stable base deployment shared among all systems\n\nWe strive to balance security and reliability with ease-of-use. In collaboration with the IU Center for Advanced Cybersecurity Research (CACR), we have developed a comprehensive set of security controls based on NIST-800-53. We support projects that work with electronically Protected Health Information (ePHI), and the bulk of these same controls are in place on all systems we operate",
    "date_created": "2010-06-01T00:00:00.000Z",
    "screenshots": [{
      "_id": "5d81137ea95efe12fcbead65",
      "caption": "Example Grafana plots for one of the SCA servers.",
      "image": "5d81137ea95efe12fcbead63"
    }],
    "__v": 10,
    "view_rank": 3,
    "logo": "5d791af50bb9b57043cb8281",
    "short_url": "ops"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }, {
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }],
  "_id": "5d80f847a95efe12fcbead07",
  "bib_string": "Young, M.D.; Hayashi, S.; Gopu, A.; Kotulla, R.; 2016. StarDock: shipping customized computing environments to the data. Proc. SPIE 9913, Software and Cyberinfrastructure for Astronomy III, 991318 (August 8, 2016); doi:10.1117/12.2233081",
  "date": null,
  "doi": "doi:10.1117/12.2233081",
  "project": "5d76b516389a4b04b4c45100",
  "links": [{
    "_id": "5d80f847a95efe12fcbead0a",
    "url": "https://www.spiedigitallibrary.org/conference-proceedings-of-spie/9913/1/StarDock-shipping-customized-computing-environments-to-the-data/10.1117/12.2233081.full",
    "label": "Online Abstract"
  }, {
    "_id": "5d80f847a95efe12fcbead09",
    "url": "https://drive.google.com/file/d/1FTyT8VPzZLSbeAT6KECbVHalf6M6Hrss/view?usp=sharing",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "5d80f847a95efe12fcbead08",
    "url": "https://drive.google.com/file/d/1p5U0ZSqM7D-NexT5me7ZbeYDsPO0E0bO/view?usp=sharing",
    "label": "Conference presentation slides (PDF)"
  }],
  "__v": 1
}, {
  "projects": [{
    "operators": ["5d24ef150a41d55c7402e029", "5d24e56b8dd3ea3f3408283d"],
    "contributors": [],
    "developers": ["5d24ba8a1c7476627c24f453", "5d82891fd0ceb47de1329ba6"],
    "leadership": ["5d24e56b8dd3ea3f3408283d"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d63ebff660730666363bf5b",
    "name": "ImageX",
    "url": "https://imagex.sca.iu.edu",
    "description": "ImageX is a set of javascript libraries used to generate and display large-scale scientific images within a web browser.  It utilizes the OpenSeaDragon open-source viewing library, and is currently deployed as part of the ODI-PPA project.",
    "date_created": "2017-10-15T00:00:00.000Z",
    "repo": "https://github.com/IUSCA/imagex",
    "logo": "5db1fd9eea2de06d5ef82053",
    "screenshots": [{
      "_id": "5d63ebff660730666363bf5f",
      "caption": "ImageX RGB colorization example",
      "image": "5d63ebff660730666363bf46"
    }, {
      "_id": "5d63ebff660730666363bf5e",
      "caption": "ImageX image details page",
      "image": "5d63ebff660730666363bf47"
    }, {
      "_id": "5d63ebff660730666363bf5d",
      "caption": "ImageX Dark Energy Camera demo",
      "image": "5d63ebff660730666363bf52"
    }],
    "__v": 6,
    "view_rank": 25,
    "short_url": "imagex"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }, {
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }],
  "_id": "5d80f8aca95efe12fcbead0f",
  "bib_string": "Hayashi, S.; Gopu, A.; Kotulla, R., Young, M.D.; 2016. Image X: new and improved image explorer for astronomical images and beyond. Proc. SPIE 9913, Software and Cyberinfrastructure for Astronomy III, 99134E (August 8, 2016); ",
  "date": null,
  "doi": "doi:10.1117/12.2233425",
  "project": "5d63ebff660730666363bf5b",
  "links": [{
    "_id": "5d80f8aca95efe12fcbead12",
    "url": "https://www.spiedigitallibrary.org/conference-proceedings-of-spie/9913/1/ImageX--new-and-improved-image-explorer-for-astronomical-images/10.1117/12.2233425.full",
    "label": "Online Abstract"
  }, {
    "_id": "5d80f8aca95efe12fcbead11",
    "url": "https://drive.google.com/file/d/1quf8LvnmNhyCAR4TuTqujhcwtg-H97td/view?usp=sharing",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "5d80f8aca95efe12fcbead10",
    "url": "https://drive.google.com/file/d/10kLClGQxCmit1czbO4YRptl_snzbVyv2/view?usp=sharing",
    "label": "Conference poster (PDF)"
  }],
  "__v": 2
}, {
  "projects": [{
    "operators": ["5d24e56b8dd3ea3f3408283d", "5d24ef150a41d55c7402e029", "5d24ba8a1c7476627c24f453"],
    "contributors": ["5d9cc2fbcb13e070e2513953", "5d9cc37ecb13e070e2513959", "5d9cc33bcb13e070e2513956"],
    "developers": ["5d24ba8a1c7476627c24f453", "5d82891fd0ceb47de1329ba6", "5d24ef660a41d55c7402e02c", "5d24e56b8dd3ea3f3408283d"],
    "leadership": ["5d24e56b8dd3ea3f3408283d", "5d828aecd0ceb47de1329ba9", "602af1bd870e9f3010f48713", "602af2c7870e9f3010f4871f", "602af287870e9f3010f4871c"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d262d7018b75a1d0b51f913",
    "name": "ODI-PPA",
    "url": "https://portal.odi.iu.edu",
    "description": "The One Degree Imager (ODI), an optical imager on the WIYN 3.5m telescope at Kitt Peak, Arizona, is designed to deliver \natmosphere-limited image quality (<0.4”) over a one degree field of view. The ODI Pipeline, Portal, and Archive (ODI-PPA) is a web science\ngateway that provides astronomers a single point of access to ODI data, and rich computational and visualization capabilities. Its goal is to\nsupport scientists in handling complex data sets, and to enhance the WIYN observatory's scientific productivity beyond data acquisition.",
    "date_created": "2010-05-03T00:00:00.000Z",
    "repo": "https://github.com/IUSCA/odi-portal/",
    "logo": "5db1fd0eea2de06d5ef8204d",
    "screenshots": [{
      "_id": "5d262d7018b75a1d0b51f917",
      "caption": "ODI-PPA Image Details page showing preview and quality assurance plot",
      "image": "5d262d7018b75a1d0b51f906"
    }, {
      "_id": "5d262d7018b75a1d0b51f916",
      "caption": "ODI-PPA homepage",
      "image": "5d262d7018b75a1d0b51f908"
    }, {
      "_id": "5d262d7018b75a1d0b51f915",
      "caption": "ODI-PPA user dashboard",
      "image": "5d262d7018b75a1d0b51f90a"
    }, {"_id": "5d262d7018b75a1d0b51f914", "caption": "ODI-PPA search page", "image": "5d262d7018b75a1d0b51f90b"}],
    "__v": 12,
    "view_rank": 2,
    "short_url": "odi"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }, {
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }],
  "_id": "5d80f94ba95efe12fcbead13",
  "bib_string": "Gopu, A.; Kotulla, R.; Young, M. D.; Hayashi, S.; Harbeck, D.; Liu, W.; Henschel, R. 2014. Rapid Large Scale Reprocessing of the ODI archive using the QuickReduce Pipeline. Proceedings of The Astronomical Society of the Pacific (ASP) 09/2015, p.53",
  "date": null,
  "doi": "",
  "project": "5d262d7018b75a1d0b51f913",
  "links": [{
    "_id": "5d80f94ba95efe12fcbead16",
    "url": "https://ui.adsabs.harvard.edu/abs/2015ASPC..495...53G/abstract",
    "label": "Online Abstract"
  }, {
    "_id": "5d80f94ba95efe12fcbead15",
    "url": "https://drive.google.com/file/d/1vCqryll2iqcrmwiYpVj2L5hjCQKpQJhA/view?usp=sharing",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "5d80f94ba95efe12fcbead14",
    "url": "https://drive.google.com/file/d/1G-CfSMvAfA2ddFiQKP8LZXZ22iJRBuCZ/view?usp=sharing",
    "label": "Conference presentation slides (PDF)"
  }],
  "__v": 1
}, {
  "projects": [{
    "operators": ["5d24e56b8dd3ea3f3408283d", "5d24ef150a41d55c7402e029", "5d24ba8a1c7476627c24f453"],
    "contributors": ["5d9cc2fbcb13e070e2513953", "5d9cc37ecb13e070e2513959", "5d9cc33bcb13e070e2513956"],
    "developers": ["5d24ba8a1c7476627c24f453", "5d82891fd0ceb47de1329ba6", "5d24ef660a41d55c7402e02c", "5d24e56b8dd3ea3f3408283d"],
    "leadership": ["5d24e56b8dd3ea3f3408283d", "5d828aecd0ceb47de1329ba9", "602af1bd870e9f3010f48713", "602af2c7870e9f3010f4871f", "602af287870e9f3010f4871c"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d262d7018b75a1d0b51f913",
    "name": "ODI-PPA",
    "url": "https://portal.odi.iu.edu",
    "description": "The One Degree Imager (ODI), an optical imager on the WIYN 3.5m telescope at Kitt Peak, Arizona, is designed to deliver \natmosphere-limited image quality (<0.4”) over a one degree field of view. The ODI Pipeline, Portal, and Archive (ODI-PPA) is a web science\ngateway that provides astronomers a single point of access to ODI data, and rich computational and visualization capabilities. Its goal is to\nsupport scientists in handling complex data sets, and to enhance the WIYN observatory's scientific productivity beyond data acquisition.",
    "date_created": "2010-05-03T00:00:00.000Z",
    "repo": "https://github.com/IUSCA/odi-portal/",
    "logo": "5db1fd0eea2de06d5ef8204d",
    "screenshots": [{
      "_id": "5d262d7018b75a1d0b51f917",
      "caption": "ODI-PPA Image Details page showing preview and quality assurance plot",
      "image": "5d262d7018b75a1d0b51f906"
    }, {
      "_id": "5d262d7018b75a1d0b51f916",
      "caption": "ODI-PPA homepage",
      "image": "5d262d7018b75a1d0b51f908"
    }, {
      "_id": "5d262d7018b75a1d0b51f915",
      "caption": "ODI-PPA user dashboard",
      "image": "5d262d7018b75a1d0b51f90a"
    }, {"_id": "5d262d7018b75a1d0b51f914", "caption": "ODI-PPA search page", "image": "5d262d7018b75a1d0b51f90b"}],
    "__v": 12,
    "view_rank": 2,
    "short_url": "odi"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }, {
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }],
  "_id": "5d80f9b4a95efe12fcbead17",
  "bib_string": "Young, M. D.; Hayashi, S.; Gopu, A.; Kotulla, R.; Harbeck, D.; Liu, W. 2014. Operational Support for Instrument Stability through ODI-PPA Metadata Visualization and Analysis. Proceedings of The Astronomical Society of the Pacific (ASP) 09/2015, p.181",
  "date": null,
  "doi": "",
  "project": "5d262d7018b75a1d0b51f913",
  "links": [{
    "_id": "5d80f9b4a95efe12fcbead1a",
    "url": "https://ui.adsabs.harvard.edu/abs/2015ASPC..495..181Y/abstract",
    "label": "Online Abstract"
  }, {
    "_id": "5d80f9b4a95efe12fcbead19",
    "url": "https://drive.google.com/file/d/1QFmMV9K1gKDoODh8qmHEVXnOma9BAhDk/view?usp=sharing",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "5d80f9b4a95efe12fcbead18",
    "url": "https://drive.google.com/file/d/1RUg8KH0Xhx-SyfMj87WwwQLjkwvlxxro/view?usp=sharing",
    "label": "Conference poster (PDF)"
  }],
  "__v": 1
}, {
  "projects": [{
    "operators": ["5d24e56b8dd3ea3f3408283d", "5d24ef150a41d55c7402e029", "5d24ba8a1c7476627c24f453"],
    "contributors": ["5d9cc2fbcb13e070e2513953", "5d9cc37ecb13e070e2513959", "5d9cc33bcb13e070e2513956"],
    "developers": ["5d24ba8a1c7476627c24f453", "5d82891fd0ceb47de1329ba6", "5d24ef660a41d55c7402e02c", "5d24e56b8dd3ea3f3408283d"],
    "leadership": ["5d24e56b8dd3ea3f3408283d", "5d828aecd0ceb47de1329ba9", "602af1bd870e9f3010f48713", "602af2c7870e9f3010f4871f", "602af287870e9f3010f4871c"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d262d7018b75a1d0b51f913",
    "name": "ODI-PPA",
    "url": "https://portal.odi.iu.edu",
    "description": "The One Degree Imager (ODI), an optical imager on the WIYN 3.5m telescope at Kitt Peak, Arizona, is designed to deliver \natmosphere-limited image quality (<0.4”) over a one degree field of view. The ODI Pipeline, Portal, and Archive (ODI-PPA) is a web science\ngateway that provides astronomers a single point of access to ODI data, and rich computational and visualization capabilities. Its goal is to\nsupport scientists in handling complex data sets, and to enhance the WIYN observatory's scientific productivity beyond data acquisition.",
    "date_created": "2010-05-03T00:00:00.000Z",
    "repo": "https://github.com/IUSCA/odi-portal/",
    "logo": "5db1fd0eea2de06d5ef8204d",
    "screenshots": [{
      "_id": "5d262d7018b75a1d0b51f917",
      "caption": "ODI-PPA Image Details page showing preview and quality assurance plot",
      "image": "5d262d7018b75a1d0b51f906"
    }, {
      "_id": "5d262d7018b75a1d0b51f916",
      "caption": "ODI-PPA homepage",
      "image": "5d262d7018b75a1d0b51f908"
    }, {
      "_id": "5d262d7018b75a1d0b51f915",
      "caption": "ODI-PPA user dashboard",
      "image": "5d262d7018b75a1d0b51f90a"
    }, {"_id": "5d262d7018b75a1d0b51f914", "caption": "ODI-PPA search page", "image": "5d262d7018b75a1d0b51f90b"}],
    "__v": 12,
    "view_rank": 2,
    "short_url": "odi"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }, {
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }],
  "_id": "5d80fa26a95efe12fcbead1b",
  "bib_string": "Liu, W.; Gopu, A.; Young, M. D.; Hayashi, S.; Kotulla, R.; Harbeck, D.; Swaters, R.; Valdes, F. 2014. Pipeline Operator Workflow for the ODI-PPA: A Novel Approach for Processing and Validating User Data. Proceedings of The Astronomical Society of the Pacific (ASP) 09/2015, p.421.",
  "date": null,
  "doi": "",
  "project": "5d262d7018b75a1d0b51f913",
  "links": [{
    "_id": "5d80fa26a95efe12fcbead1e",
    "url": "https://drive.google.com/file/d/1Haqiy0XKi9OOurpSsqIeDNTMRD1i6qS3/view?usp=sharing",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "5d80fa26a95efe12fcbead1d",
    "url": "https://drive.google.com/file/d/11803hZAUDz-1yUxg38IVNb4BR5O2Z92K/view?usp=sharing",
    "label": "Conference poster (PDF)"
  }, {"_id": "5d80fa26a95efe12fcbead1c", "url": "", "label": ""}],
  "__v": 1
}, {
  "projects": [{
    "operators": ["5d24e56b8dd3ea3f3408283d", "5d24ef150a41d55c7402e029", "5d24ba8a1c7476627c24f453"],
    "contributors": ["5d9cc2fbcb13e070e2513953", "5d9cc37ecb13e070e2513959", "5d9cc33bcb13e070e2513956"],
    "developers": ["5d24ba8a1c7476627c24f453", "5d82891fd0ceb47de1329ba6", "5d24ef660a41d55c7402e02c", "5d24e56b8dd3ea3f3408283d"],
    "leadership": ["5d24e56b8dd3ea3f3408283d", "5d828aecd0ceb47de1329ba9", "602af1bd870e9f3010f48713", "602af2c7870e9f3010f4871f", "602af287870e9f3010f4871c"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d262d7018b75a1d0b51f913",
    "name": "ODI-PPA",
    "url": "https://portal.odi.iu.edu",
    "description": "The One Degree Imager (ODI), an optical imager on the WIYN 3.5m telescope at Kitt Peak, Arizona, is designed to deliver \natmosphere-limited image quality (<0.4”) over a one degree field of view. The ODI Pipeline, Portal, and Archive (ODI-PPA) is a web science\ngateway that provides astronomers a single point of access to ODI data, and rich computational and visualization capabilities. Its goal is to\nsupport scientists in handling complex data sets, and to enhance the WIYN observatory's scientific productivity beyond data acquisition.",
    "date_created": "2010-05-03T00:00:00.000Z",
    "repo": "https://github.com/IUSCA/odi-portal/",
    "logo": "5db1fd0eea2de06d5ef8204d",
    "screenshots": [{
      "_id": "5d262d7018b75a1d0b51f917",
      "caption": "ODI-PPA Image Details page showing preview and quality assurance plot",
      "image": "5d262d7018b75a1d0b51f906"
    }, {
      "_id": "5d262d7018b75a1d0b51f916",
      "caption": "ODI-PPA homepage",
      "image": "5d262d7018b75a1d0b51f908"
    }, {
      "_id": "5d262d7018b75a1d0b51f915",
      "caption": "ODI-PPA user dashboard",
      "image": "5d262d7018b75a1d0b51f90a"
    }, {"_id": "5d262d7018b75a1d0b51f914", "caption": "ODI-PPA search page", "image": "5d262d7018b75a1d0b51f90b"}],
    "__v": 12,
    "view_rank": 2,
    "short_url": "odi"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }, {
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }],
  "_id": "5d80fa75a95efe12fcbead1f",
  "bib_string": "Gopu, A.; Hayashi, S.; Young, M. D.; Harbeck, D.; Boroson, T.; Liu, W.; Kotulla, R.; Shaw, R.; Henschel, R.; Rajagopal, J.; Stobie, E.; Knezek, P.; Martin, P.; Archbold, K. 2014. ODI - Portal, Pipeline, and Archive (ODI-PPA): a web-based astronomical compute archive, visualization, and analysis service. Proc. SPIE 9152, Software and Cyberinfrastructure for Astronomy III, 91520E (July 18, 2014); ",
  "date": null,
  "doi": "doi:10.1117/12.2057123",
  "project": "5d262d7018b75a1d0b51f913",
  "links": [{
    "_id": "5d80fa75a95efe12fcbead22",
    "url": "https://www.spiedigitallibrary.org/conference-proceedings-of-spie/9152/1/ODI---Portal-Pipeline-and-Archive-ODI-PPA/10.1117/12.2057123.full",
    "label": "Online Abstract"
  }, {
    "_id": "5d80fa75a95efe12fcbead21",
    "url": "https://drive.google.com/file/d/1Fc4uHvj1Ou3Vl-OkJSG7gv58kTY1Nr2H/view?usp=sharing",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "5d80fa75a95efe12fcbead20",
    "url": "https://drive.google.com/file/d/1CuWC8w1OYl6Br1d-_6HaSV3cre8zps5m/view?usp=sharing",
    "label": "Conference presentation slides (PDF)"
  }],
  "__v": 1
}, {
  "projects": [{
    "operators": ["5d24e56b8dd3ea3f3408283d", "5d24ef150a41d55c7402e029", "5d24ba8a1c7476627c24f453"],
    "contributors": ["5d9cc2fbcb13e070e2513953", "5d9cc37ecb13e070e2513959", "5d9cc33bcb13e070e2513956"],
    "developers": ["5d24ba8a1c7476627c24f453", "5d82891fd0ceb47de1329ba6", "5d24ef660a41d55c7402e02c", "5d24e56b8dd3ea3f3408283d"],
    "leadership": ["5d24e56b8dd3ea3f3408283d", "5d828aecd0ceb47de1329ba9", "602af1bd870e9f3010f48713", "602af2c7870e9f3010f4871f", "602af287870e9f3010f4871c"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d262d7018b75a1d0b51f913",
    "name": "ODI-PPA",
    "url": "https://portal.odi.iu.edu",
    "description": "The One Degree Imager (ODI), an optical imager on the WIYN 3.5m telescope at Kitt Peak, Arizona, is designed to deliver \natmosphere-limited image quality (<0.4”) over a one degree field of view. The ODI Pipeline, Portal, and Archive (ODI-PPA) is a web science\ngateway that provides astronomers a single point of access to ODI data, and rich computational and visualization capabilities. Its goal is to\nsupport scientists in handling complex data sets, and to enhance the WIYN observatory's scientific productivity beyond data acquisition.",
    "date_created": "2010-05-03T00:00:00.000Z",
    "repo": "https://github.com/IUSCA/odi-portal/",
    "logo": "5db1fd0eea2de06d5ef8204d",
    "screenshots": [{
      "_id": "5d262d7018b75a1d0b51f917",
      "caption": "ODI-PPA Image Details page showing preview and quality assurance plot",
      "image": "5d262d7018b75a1d0b51f906"
    }, {
      "_id": "5d262d7018b75a1d0b51f916",
      "caption": "ODI-PPA homepage",
      "image": "5d262d7018b75a1d0b51f908"
    }, {
      "_id": "5d262d7018b75a1d0b51f915",
      "caption": "ODI-PPA user dashboard",
      "image": "5d262d7018b75a1d0b51f90a"
    }, {"_id": "5d262d7018b75a1d0b51f914", "caption": "ODI-PPA search page", "image": "5d262d7018b75a1d0b51f90b"}],
    "__v": 12,
    "view_rank": 2,
    "short_url": "odi"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }, {
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }],
  "_id": "5d80fb76a95efe12fcbead2b",
  "bib_string": "Young, M. D.; Kotulla, R.; Gopu, A.; Liu, W. 2014. Integrating the ODI-PPA scientific gateway with the QuickReduce pipeline for on-demand processing. Proc. SPIE 9152, Software and Cyberinfrastructure for Astronomy III, 91522U (July 18, 2014)",
  "date": null,
  "doi": "doi:10.1117/12.2056763",
  "project": "5d262d7018b75a1d0b51f913",
  "links": [{
    "_id": "5d80fb76a95efe12fcbead2e",
    "url": "https://www.spiedigitallibrary.org/conference-proceedings-of-spie/9152/1/Integrating-the-ODI-PPA-scientific-gateway-with-the-QuickReduce-pipeline/10.1117/12.2056763.full",
    "label": "Online Abstract"
  }, {
    "_id": "5d80fb76a95efe12fcbead2d",
    "url": "https://drive.google.com/file/d/1LoYSwxSbiIupmpVDeN66xAXfQS1Dxwst/view?usp=sharing",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "5d80fb76a95efe12fcbead2c",
    "url": "https://drive.google.com/file/d/1QE4qqyJQMpv2ILn8tVx9ipJZe0pROTOZ/view?usp=sharing",
    "label": "Conference poster (PDF)"
  }],
  "__v": 1
}, {
  "projects": [{
    "operators": ["5d24e56b8dd3ea3f3408283d", "5d24ef150a41d55c7402e029", "5d24ba8a1c7476627c24f453"],
    "contributors": ["5d9cc2fbcb13e070e2513953", "5d9cc37ecb13e070e2513959", "5d9cc33bcb13e070e2513956"],
    "developers": ["5d24ba8a1c7476627c24f453", "5d82891fd0ceb47de1329ba6", "5d24ef660a41d55c7402e02c", "5d24e56b8dd3ea3f3408283d"],
    "leadership": ["5d24e56b8dd3ea3f3408283d", "5d828aecd0ceb47de1329ba9", "602af1bd870e9f3010f48713", "602af2c7870e9f3010f4871f", "602af287870e9f3010f4871c"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d262d7018b75a1d0b51f913",
    "name": "ODI-PPA",
    "url": "https://portal.odi.iu.edu",
    "description": "The One Degree Imager (ODI), an optical imager on the WIYN 3.5m telescope at Kitt Peak, Arizona, is designed to deliver \natmosphere-limited image quality (<0.4”) over a one degree field of view. The ODI Pipeline, Portal, and Archive (ODI-PPA) is a web science\ngateway that provides astronomers a single point of access to ODI data, and rich computational and visualization capabilities. Its goal is to\nsupport scientists in handling complex data sets, and to enhance the WIYN observatory's scientific productivity beyond data acquisition.",
    "date_created": "2010-05-03T00:00:00.000Z",
    "repo": "https://github.com/IUSCA/odi-portal/",
    "logo": "5db1fd0eea2de06d5ef8204d",
    "screenshots": [{
      "_id": "5d262d7018b75a1d0b51f917",
      "caption": "ODI-PPA Image Details page showing preview and quality assurance plot",
      "image": "5d262d7018b75a1d0b51f906"
    }, {
      "_id": "5d262d7018b75a1d0b51f916",
      "caption": "ODI-PPA homepage",
      "image": "5d262d7018b75a1d0b51f908"
    }, {
      "_id": "5d262d7018b75a1d0b51f915",
      "caption": "ODI-PPA user dashboard",
      "image": "5d262d7018b75a1d0b51f90a"
    }, {"_id": "5d262d7018b75a1d0b51f914", "caption": "ODI-PPA search page", "image": "5d262d7018b75a1d0b51f90b"}],
    "__v": 12,
    "view_rank": 2,
    "short_url": "odi"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }, {
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }],
  "_id": "5d80fbe3a95efe12fcbead2f",
  "bib_string": "Gopu, A.; Hayashi, S.; Young, M. D. 2013. Image Explorer: Astronomical Image Analysis on an HTML5-based Web Application. In ASP Conference Series Volume 485, Page 417, Astronomical Data Analysis Software and Systems XXIII",
  "date": null,
  "doi": "",
  "project": "5d262d7018b75a1d0b51f913",
  "links": [{
    "_id": "5d80fbe3a95efe12fcbead32",
    "url": "http://www.aspbooks.org/a/volumes/article_details/?paper_id=36264",
    "label": "Online Abstract"
  }, {
    "_id": "5d80fbe3a95efe12fcbead31",
    "url": "https://drive.google.com/file/d/1hHtHzKT6Ne3b0Cv_O7-1Q3ETkjk7HSPM/view?usp=sharing",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "5d80fbe3a95efe12fcbead30",
    "url": "https://drive.google.com/file/d/1qj7ZC9Xcdm1etJceDfGJNPZSe1wWsl4A/view?usp=sharing",
    "label": "Conference presentation slides (PDF)"
  }],
  "__v": 1
}, {
  "projects": [{
    "operators": ["5d24e56b8dd3ea3f3408283d", "5d24ef150a41d55c7402e029", "5d24ba8a1c7476627c24f453"],
    "contributors": ["5d9cc2fbcb13e070e2513953", "5d9cc37ecb13e070e2513959", "5d9cc33bcb13e070e2513956"],
    "developers": ["5d24ba8a1c7476627c24f453", "5d82891fd0ceb47de1329ba6", "5d24ef660a41d55c7402e02c", "5d24e56b8dd3ea3f3408283d"],
    "leadership": ["5d24e56b8dd3ea3f3408283d", "5d828aecd0ceb47de1329ba9", "602af1bd870e9f3010f48713", "602af2c7870e9f3010f4871f", "602af287870e9f3010f4871c"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d262d7018b75a1d0b51f913",
    "name": "ODI-PPA",
    "url": "https://portal.odi.iu.edu",
    "description": "The One Degree Imager (ODI), an optical imager on the WIYN 3.5m telescope at Kitt Peak, Arizona, is designed to deliver \natmosphere-limited image quality (<0.4”) over a one degree field of view. The ODI Pipeline, Portal, and Archive (ODI-PPA) is a web science\ngateway that provides astronomers a single point of access to ODI data, and rich computational and visualization capabilities. Its goal is to\nsupport scientists in handling complex data sets, and to enhance the WIYN observatory's scientific productivity beyond data acquisition.",
    "date_created": "2010-05-03T00:00:00.000Z",
    "repo": "https://github.com/IUSCA/odi-portal/",
    "logo": "5db1fd0eea2de06d5ef8204d",
    "screenshots": [{
      "_id": "5d262d7018b75a1d0b51f917",
      "caption": "ODI-PPA Image Details page showing preview and quality assurance plot",
      "image": "5d262d7018b75a1d0b51f906"
    }, {
      "_id": "5d262d7018b75a1d0b51f916",
      "caption": "ODI-PPA homepage",
      "image": "5d262d7018b75a1d0b51f908"
    }, {
      "_id": "5d262d7018b75a1d0b51f915",
      "caption": "ODI-PPA user dashboard",
      "image": "5d262d7018b75a1d0b51f90a"
    }, {"_id": "5d262d7018b75a1d0b51f914", "caption": "ODI-PPA search page", "image": "5d262d7018b75a1d0b51f90b"}],
    "__v": 12,
    "view_rank": 2,
    "short_url": "odi"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }, {
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }],
  "_id": "5d80fc16a95efe12fcbead33",
  "bib_string": "Young, M. D.; Gopu, A.; Hayashi, S. 2013. Source Explorer: Towards web-browser based tools for astronomical source visualization and analysis. In ASP Conference Series Volume 485, Page 269, Astronomical Data Analysis Software and Systems XXIII",
  "date": null,
  "doi": "",
  "project": "5d262d7018b75a1d0b51f913",
  "links": [{
    "_id": "5d80fc16a95efe12fcbead36",
    "url": "http://www.aspbooks.org/a/volumes/article_details/?paper_id=36229",
    "label": "Online Abstract"
  }, {
    "_id": "5d80fc16a95efe12fcbead35",
    "url": "https://drive.google.com/file/d/1Q_sS6BvsK_HSmanviAao1LqHr5P-Danc/view?usp=sharing",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "5d80fc16a95efe12fcbead34",
    "url": "https://drive.google.com/file/d/1qj7ZC9Xcdm1etJceDfGJNPZSe1wWsl4A/view?usp=sharing",
    "label": "Conference presentation slides (PDF)"
  }],
  "__v": 1
}, {
  "projects": [{
    "operators": ["5d24e56b8dd3ea3f3408283d", "5d24ef150a41d55c7402e029", "5d24ba8a1c7476627c24f453"],
    "contributors": ["5d9cc2fbcb13e070e2513953", "5d9cc37ecb13e070e2513959", "5d9cc33bcb13e070e2513956"],
    "developers": ["5d24ba8a1c7476627c24f453", "5d82891fd0ceb47de1329ba6", "5d24ef660a41d55c7402e02c", "5d24e56b8dd3ea3f3408283d"],
    "leadership": ["5d24e56b8dd3ea3f3408283d", "5d828aecd0ceb47de1329ba9", "602af1bd870e9f3010f48713", "602af2c7870e9f3010f4871f", "602af287870e9f3010f4871c"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d262d7018b75a1d0b51f913",
    "name": "ODI-PPA",
    "url": "https://portal.odi.iu.edu",
    "description": "The One Degree Imager (ODI), an optical imager on the WIYN 3.5m telescope at Kitt Peak, Arizona, is designed to deliver \natmosphere-limited image quality (<0.4”) over a one degree field of view. The ODI Pipeline, Portal, and Archive (ODI-PPA) is a web science\ngateway that provides astronomers a single point of access to ODI data, and rich computational and visualization capabilities. Its goal is to\nsupport scientists in handling complex data sets, and to enhance the WIYN observatory's scientific productivity beyond data acquisition.",
    "date_created": "2010-05-03T00:00:00.000Z",
    "repo": "https://github.com/IUSCA/odi-portal/",
    "logo": "5db1fd0eea2de06d5ef8204d",
    "screenshots": [{
      "_id": "5d262d7018b75a1d0b51f917",
      "caption": "ODI-PPA Image Details page showing preview and quality assurance plot",
      "image": "5d262d7018b75a1d0b51f906"
    }, {
      "_id": "5d262d7018b75a1d0b51f916",
      "caption": "ODI-PPA homepage",
      "image": "5d262d7018b75a1d0b51f908"
    }, {
      "_id": "5d262d7018b75a1d0b51f915",
      "caption": "ODI-PPA user dashboard",
      "image": "5d262d7018b75a1d0b51f90a"
    }, {"_id": "5d262d7018b75a1d0b51f914", "caption": "ODI-PPA search page", "image": "5d262d7018b75a1d0b51f90b"}],
    "__v": 12,
    "view_rank": 2,
    "short_url": "odi"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }, {
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }],
  "_id": "5d80fc46a95efe12fcbead37",
  "bib_string": "Young, M. D.; Gopu, A.; Hayashi, S.; Cox, J. A. 2012. FRIAA: A FRamework for Web-based Interactive Astronomy Analysis using AMQP Messaging. In ASP Conference Series Volume 475, Page 337, Astronomical Data Analysis Software and Systems XXII",
  "date": null,
  "doi": "",
  "project": "5d262d7018b75a1d0b51f913",
  "links": [{
    "_id": "5d80fc46a95efe12fcbead3a",
    "url": "http://www.aspbooks.org/a/volumes/article_details/?paper_id=35634",
    "label": "Online Abstract"
  }, {
    "_id": "5d80fc46a95efe12fcbead39",
    "url": "https://drive.google.com/file/d/1uZgbU0FLGTVMMO9QHKUzNXUKc-y0E9IH/view?usp=sharing",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "5d80fc46a95efe12fcbead38",
    "url": "https://drive.google.com/file/d/1tBpwaXyzGFCZsy1GVKri8skDhH9ptHjQ/view?usp=sharing",
    "label": "Conference presentation slides (PDF)"
  }],
  "__v": 1
}, {
  "projects": [{
    "operators": ["5d24e56b8dd3ea3f3408283d", "5d24ef150a41d55c7402e029"],
    "contributors": [],
    "developers": ["5d24ba8a1c7476627c24f453"],
    "leadership": ["5d24e56b8dd3ea3f3408283d", "602af1bd870e9f3010f48713"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d6010f6c55df811d919ca52",
    "name": "SpArc",
    "url": "https://sparc.sca.iu.edu",
    "description": "The data in this archive was gathered on the Kitt Peak National Observatory’s Mayall 4m telescope taken with the Fourier Transform Spectrometer (FTS) during the period from 1975-1995. The FTS produced spectra in the wavelength regime from roughly 0.9 to 5 microns (11,000 to 2000 cm-1), mostly at relatively high spectral resolution. The FTS was developed and maintained at Kitt Peak by Donald Hall, Stephen Ridgway, and Kenneth Hinkle (Hall et al. 1979), in partnership with the solar FTS at the McMath-Pierce Solar Telescope, developed by James Brault1.\n\nDuring this period (before the development and deployment of infrared arrays), an FTS permitted observations of infrared spectra that could not be obtained any other way. More than 800 targets were observed with the 4-m FTS, many of them multiple times. Targets observed by numerous individual investigators include a variety of normal and peculiar red giants, solar type stars, M dwarfs, variable stars, and early type stars (for telluric line removal) as well as nebulae and galaxies. Observations were limited to a magnitude of K=4 or brighter at R>20,000, although some fainter targets were included at lower resolution. The spectra generally cover a relatively wide wavelength range within the J, H, K, L, or M atmospheric window, and FTS spectrometers provide the advantage of a very clean line profile compared to traditional spectrographs.",
    "date_created": "2016-05-30T00:00:00.000Z",
    "repo": "https://github.iu.edu/SpArc",
    "logo": "5d6010f6c55df811d919ca44",
    "screenshots": [{
      "_id": "5d6010f6c55df811d919ca55",
      "caption": "Caption Test",
      "image": "5d6010f6c55df811d919ca45"
    }, {
      "_id": "5d6010f6c55df811d919ca54",
      "caption": "Caption Test",
      "image": "5d6010f6c55df811d919ca48"
    }, {"_id": "5d6010f6c55df811d919ca53", "caption": "Caption Test", "image": "5d6010f6c55df811d919ca4d"}],
    "__v": 5,
    "view_rank": 17,
    "short_url": "sparc"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }, {
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }],
  "_id": "5d80fd19a95efe12fcbead3e",
  "bib_string": "Pilachowski, C.A.; Hinkle, K.H.; Young, M.D.; Dennis, H.B.; Gopu, A.; Henschel, R.; Hayashi, S. 2017. An Archive of Spectra from the Mayall Fourier Transform Spectrometer at Kitt Peak. Journal: Publications of the Astronomical Society of the Pacific}, volume 129, number 972; arXiv:1610.02535 [astro-ph.IM]",
  "date": null,
  "doi": "arXiv:1610.02535",
  "project": "5d6010f6c55df811d919ca52",
  "links": [{
    "_id": "5d80fd19a95efe12fcbead40",
    "url": "https://ui.adsabs.harvard.edu/abs/2017PASP..129b4006P",
    "label": "Online Abstract"
  }, {"_id": "5d80fd19a95efe12fcbead3f", "url": "https://arxiv.org/pdf/1610.02535.pdf", "label": "Full paper (PDF)"}],
  "__v": 0
}, {
  "projects": [{
    "operators": ["5d24e56b8dd3ea3f3408283d", "5d24ef150a41d55c7402e029"],
    "contributors": [],
    "developers": ["5d24ba8a1c7476627c24f453"],
    "leadership": ["5d24e56b8dd3ea3f3408283d", "602af1bd870e9f3010f48713"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d6010f6c55df811d919ca52",
    "name": "SpArc",
    "url": "https://sparc.sca.iu.edu",
    "description": "The data in this archive was gathered on the Kitt Peak National Observatory’s Mayall 4m telescope taken with the Fourier Transform Spectrometer (FTS) during the period from 1975-1995. The FTS produced spectra in the wavelength regime from roughly 0.9 to 5 microns (11,000 to 2000 cm-1), mostly at relatively high spectral resolution. The FTS was developed and maintained at Kitt Peak by Donald Hall, Stephen Ridgway, and Kenneth Hinkle (Hall et al. 1979), in partnership with the solar FTS at the McMath-Pierce Solar Telescope, developed by James Brault1.\n\nDuring this period (before the development and deployment of infrared arrays), an FTS permitted observations of infrared spectra that could not be obtained any other way. More than 800 targets were observed with the 4-m FTS, many of them multiple times. Targets observed by numerous individual investigators include a variety of normal and peculiar red giants, solar type stars, M dwarfs, variable stars, and early type stars (for telluric line removal) as well as nebulae and galaxies. Observations were limited to a magnitude of K=4 or brighter at R>20,000, although some fainter targets were included at lower resolution. The spectra generally cover a relatively wide wavelength range within the J, H, K, L, or M atmospheric window, and FTS spectrometers provide the advantage of a very clean line profile compared to traditional spectrographs.",
    "date_created": "2016-05-30T00:00:00.000Z",
    "repo": "https://github.iu.edu/SpArc",
    "logo": "5d6010f6c55df811d919ca44",
    "screenshots": [{
      "_id": "5d6010f6c55df811d919ca55",
      "caption": "Caption Test",
      "image": "5d6010f6c55df811d919ca45"
    }, {
      "_id": "5d6010f6c55df811d919ca54",
      "caption": "Caption Test",
      "image": "5d6010f6c55df811d919ca48"
    }, {"_id": "5d6010f6c55df811d919ca53", "caption": "Caption Test", "image": "5d6010f6c55df811d919ca4d"}],
    "__v": 5,
    "view_rank": 17,
    "short_url": "sparc"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }, {
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }],
  "_id": "5d80fd4da95efe12fcbead41",
  "bib_string": "Young M. D.; Pilachowski, C.A.; Dennis., H.B.; Gopu, A.; 2016. SpArc: Preservation of 20 years of Spectrographic Data. ADASS2016, Italy.",
  "date": null,
  "doi": "",
  "project": "5d6010f6c55df811d919ca52",
  "links": [{
    "_id": "5d80fd4da95efe12fcbead44",
    "url": "http://www.adass2016.inaf.it/index.php/participants-all/4-poster/70-young-michael",
    "label": "Online Abstract"
  }, {
    "_id": "5d80fd4da95efe12fcbead43",
    "url": "https://drive.google.com/file/d/111JaKEyrYPubU4xMbFN4xp4mdpUhcURE/view?usp=sharing",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "5d80fd4da95efe12fcbead42",
    "url": "https://drive.google.com/file/d/1Ctw53v8Dfonpa-fjh0YAGiDOiDf3mAEA/view?usp=sharing",
    "label": "Conference poster (PDF)"
  }],
  "__v": 1
}, {
  "projects": [{
    "operators": ["5d24e56b8dd3ea3f3408283d", "5d24ef150a41d55c7402e029"],
    "contributors": [],
    "developers": ["5d24ba8a1c7476627c24f453", "5d24e56b8dd3ea3f3408283d"],
    "leadership": ["5d24e56b8dd3ea3f3408283d", "5d828aecd0ceb47de1329ba9"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d7126674db0c0676e56cdd7",
    "name": "EMC-SCA",
    "url": "n/a",
    "description": "Groups from the IU-Bloomington Electron Microscopy Center (EMC) and Pervasive Technology Institute (PTI)  created a project to deal with the tidal wave of images produced using EMC resources. The EMC SCA is an offshoot of a project for handling images from the One Degree Imager on the WIYN 3.5m telescope at Kitt Peak, Arizona. The concept behind both projects is that images are uploaded from the recording instrument(s) into a database that is archival and searchable. Images are stored with calibration and reference data, instrument metadata and tag words to help users search for particular images. Access control exists for the images. The images and all functions of the database are accessible through any internet browser. Images are stored locally on the Data Capacitor shared file system and archivally in the Scholarly Data Archive (SDA). A number-crunching pipeline built on the Big Red II computing cluster is used for compute-intensive data reduction and image processing.",
    "date_created": "2014-04-01T00:00:00.000Z",
    "repo": "https://github.iu.edu/emcenter",
    "logo": "5d791cdb0bb9b57043cb8289",
    "screenshots": [{
      "_id": "5d7126674db0c0676e56cdd9",
      "caption": "EMC-SCA image collection preview",
      "image": "5d7126674db0c0676e56cdcf"
    }, {"_id": "5d7126674db0c0676e56cdd8", "caption": "EMC-SCA search page", "image": "5d7126674db0c0676e56cdd0"}],
    "__v": 6,
    "view_rank": 31,
    "short_url": "emc",
    "date_retired": "2019-03-31T00:00:00.000Z"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }, {
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }],
  "_id": "5d80fd6aa95efe12fcbead45",
  "bib_string": "Morgan, D.; Gopu, A.; Young, M.D.; Hayashi, S. 2014. EMC-SCA: Organizing, Managing and Searching Large Collections of Images: A New Resource To Handle High-Throughput Imaging. Oral Presentation, Proceedings of 18th International Microscopy Congress, Prague, Czech Republic.",
  "date": null,
  "doi": "",
  "project": "5d7126674db0c0676e56cdd7",
  "links": [{
    "_id": "5d80fd6aa95efe12fcbead46",
    "url": "http://www.microscopy.cz/html/3387.html",
    "label": "Online Abstract"
  }],
  "__v": 0
}, {
  "projects": [{
    "operators": ["5d24e56b8dd3ea3f3408283d", "5d24ef150a41d55c7402e029"],
    "contributors": [],
    "developers": ["5d24ba8a1c7476627c24f453", "5d24e5908dd3ea3f34082840", "5d82891fd0ceb47de1329ba6"],
    "leadership": ["5d24e56b8dd3ea3f3408283d", "5d24ba8a1c7476627c24f453"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d260b675895982d259d31f4",
    "name": "SQAN",
    "url": "https://sqan.sca.iu.edu",
    "description": "Medical imaging, a key component in clinical diagnosis of and research on numerous medical conditions, is very costly and can generate massive datasets. For instance, a single scanned subject produces hundreds of thousands of images and millions of key-value metadata pairs that must be verified to ensure instrument and research protocol compliance. Many projects lack funds to reacquire images if data quality issues are detected later. Data quality assurance (QA) requires continuous involvement by all stakeholders and use of specific quality control (QC) methods to identify data issues likely to require post-processing correction or real-time re-acquisition. While many useful QC methods exist, they are often designed for specific use-cases with limited scope and documentation, making integration with other setups difficult. We present the Scalable Quality Assurance for Neuroimaging (SQAN), an open-source software suite developed by Indiana University for protocol quality control and instrumental validation on medical imaging data. SQAN includes a comprehensive QC Engine that ensures adherence to a research study’s protocol. A modern, intuitive web portal serves a wide range of users including researchers, scanner technologists and data scientists, each of whom approach QC with unique priorities, expertise, insights and expectations. Since Fall 2017, a fully operational SQAN instance has supported 50+ research projects, and has QC’d ∼4 million images and over 1000 million metadata tags. SQAN is designed to scale to any imaging center’s QC needs, and to extend beyond protocol QC toward image-level QC and integration with pipeline and non-imaging database systems.\n",
    "date_created": "2015-06-01T00:00:00.000Z",
    "repo": "https://github.com/IUSCA/SQAN/",
    "logo": "5db1fdfaea2de06d5ef82058",
    "screenshots": [{
      "_id": "5d260b675895982d259d31f7",
      "caption": "SQAN provides detailed QA messages for series and individual images",
      "image": "5d260b675895982d259d31ed"
    }, {
      "_id": "5d260b675895982d259d31f6",
      "caption": "Intuitive feedback at the subject/exam level",
      "image": "5d260b675895982d259d31ef"
    }, {
      "_id": "5d260b675895982d259d31f5",
      "caption": "Overall summary provided for project researchers",
      "image": "5d260b675895982d259d31f1"
    }],
    "__v": 24,
    "view_rank": 4,
    "short_url": "sqan"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24e56b8dd3ea3f3408283d",
    "role": "Team Manager",
    "name": "Arvind Gopu",
    "email": "agopu@iu.edu",
    "headshot": "60f5d09d82d1976bd987d2af",
    "__v": 0,
    "background": "MS in Computer Science (IU 2004)",
    "joined": "2010-05-01T00:00:00.000Z",
    "sca": true,
    "uid": "agopu",
    "view_rank": 1
  }, {
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }, {
    "active": true,
    "_id": "5d24e5908dd3ea3f34082840",
    "role": "Senior Analyst Programmer",
    "name": "Andrea Conway",
    "email": "aiavenak@iu.edu",
    "headshot": "5d24e5908dd3ea3f3408283e",
    "__v": 0,
    "background": "Ph.D in Neuroscience and Psychology",
    "joined": "2018-05-14T00:00:00.000Z",
    "sca": true,
    "uid": "aiavenak",
    "view_rank": 4
  }, {
    "active": true,
    "_id": "5d24ef150a41d55c7402e029",
    "role": "Operations Lead",
    "name": "Raymond Perigo",
    "email": "rperigo@iu.edu",
    "headshot": "6244731c0f3fcc2f7573ec35",
    "__v": 0,
    "background": "RHCE Certification",
    "joined": "2016-07-01T00:00:00.000Z",
    "sca": true,
    "uid": "rperigo",
    "view_rank": 3
  }, {
    "active": false,
    "_id": "5d9cd548cb13e070e251396b",
    "name": "John West",
    "email": "jdwest@iu.edu",
    "role": "Late Collaborator",
    "background": "John West worked for the Center for Neuroimaging and Indiana Alzheimers Disease Center.  His duties included processing/analysis of research imaging datasets, archiving/databasing of imaging & genetics data, and general IT support for center faculty, students and staff. John passed away unexpectedly on Oct 17 2020 - he will certainly be missed.",
    "joined": null,
    "sca": false,
    "view_rank": 6,
    "headshot": "5f4561c00991df19c3a9a9c6",
    "__v": 0,
    "uid": "jdwest"
  }, {
    "active": true,
    "_id": "5e4713c3b217fd09d24177dc",
    "name": "Sundar Paramasivam",
    "email": "mparamas@iu.edu",
    "role": "Collaborator",
    "background": "Sundar works for the Indy based RADY imaging center.",
    "joined": null,
    "sca": false,
    "view_rank": 9,
    "headshot": "5e4713fdb217fd09d24177dd",
    "__v": 0,
    "uid": "mparamas"
  }, {
    "active": false,
    "_id": "5d82891fd0ceb47de1329ba6",
    "name": "Soichi Hayashi",
    "email": "hayashis@iu.edu",
    "role": "Former Lead Developer",
    "background": "Contributed key foundational components to the ODI project since its inception. Technical lead developer between 2014-2016.",
    "joined": "2010-05-01T00:00:00.000Z",
    "headshot": "5d82891fd0ceb47de1329ba4",
    "__v": 0,
    "sca": true,
    "view_rank": 3,
    "uid": "hayashis",
    "left": "2017-06-30T00:00:00.000Z"
  }, {
    "active": true,
    "_id": "5d828aecd0ceb47de1329ba9",
    "name": "Robert Henschel",
    "email": "henschel@iu.edu",
    "role": "Former Director, Research and Software Solutions",
    "background": "Research project liaison and advisor starting Oct 2021. Formerly Director of RSS July 2016 - Sep 2021. MS in Computer Science. ",
    "joined": "2010-05-01T00:00:00.000Z",
    "headshot": "5d828aecd0ceb47de1329ba7",
    "__v": 0,
    "sca": false,
    "view_rank": 0,
    "uid": "henshel"
  }],
  "_id": "5d80fe15a95efe12fcbead49",
  "bib_string": "Gopu, A., Young, M. D., Avena-Koenigsberger, A., Perigo, R., West, J., Paramasivam, M., Hayashi, S., Henschel, R. Scalable Quality Assurance for Neuroimaging (SQAN): automated quality control for medical imaging, Proc. SPIE 11318, Medical Imaging 2020: Imaging Informatics for Healthcare, Research, and Applications, 1131807 (2 March 2020); https://doi.org/10.1117/12.2549722",
  "date": null,
  "doi": "",
  "project": "5d260b675895982d259d31f4",
  "links": [{
    "_id": "5e49962fb217fd09d24177e1",
    "url": "https://www.spiedigitallibrary.org/conference-proceedings-of-spie/11318/1131807/Scalable-Quality-Assurance-for-Neuroimaging-SQAN--automated-quality-control/10.1117/12.2549722.short",
    "label": "Online Abstract (PDF)"
  }, {
    "_id": "5e49962fb217fd09d24177e0",
    "url": "https://drive.google.com/file/d/1YFqtNp2HfrMUHq79XXIBDz2Ej3CRU-z0/view?usp=sharing",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "5e49962fb217fd09d24177df",
    "url": "https://drive.google.com/file/d/1PUPeMKcEzM1ZUA6KUZY7JzB72xKHn7RE/view?usp=sharing",
    "label": "Conference Presentation Slides (PDF)"
  }, {
    "_id": "5e499660b217fd09d24177e2",
    "url": "https://drive.google.com/file/d/1n1kzFy6Z3WkVM_VNoDo7Z9-BnWgjYHaV/view?usp=sharing",
    "label": "Live Workshop Handout (PDF)"
  }],
  "__v": 7
}, {
  "projects": [{
    "operators": ["5d24ef150a41d55c7402e029", "5d24e56b8dd3ea3f3408283d"],
    "contributors": [],
    "developers": ["5d24ba8a1c7476627c24f453"],
    "leadership": ["602af1bd870e9f3010f48713", "5d9cc2c1cb13e070e2513950", "5d24e56b8dd3ea3f3408283d"],
    "publications": [],
    "funding": [],
    "languages": [],
    "_id": "5d63e98f660730666363bf31",
    "name": "BDBS-SCA",
    "url": "https://bdbs.sca.iu.edu",
    "description": "The Blanco DECam Bulge Survey (BDBS), a three-year NSF-funded project, alleviates these difficulties by creating images of approximately 200 square degrees of the Milky Way galaxy’s bulge region. To do so, the project used the Dark Energy Camera (DECam) attached to the Blanco 4m Telescope at the Cerro Tololo Inter-American Observatory in Chile. ",
    "date_created": "2015-02-15T00:00:00.000Z",
    "repo": "https://github.iu.edu/youngmd/BDBS",
    "logo": "5d63e98f660730666363bf11",
    "screenshots": [{
      "_id": "5d63e98f660730666363bf34",
      "caption": "BDBS Job Page",
      "image": "5d63e98f660730666363bf12"
    }, {
      "_id": "5d63e98f660730666363bf33",
      "caption": "BDBS Search Page",
      "image": "5d63e98f660730666363bf14"
    }, {"_id": "5d63e98f660730666363bf32", "caption": "BDBS Home Page", "image": "5d63e98f660730666363bf15"}],
    "__v": 5,
    "view_rank": 18,
    "short_url": "bdbs"
  }],
  "authors": [{
    "active": true,
    "_id": "5d24ba8a1c7476627c24f453",
    "role": "Lead Software Developer",
    "name": "Michael Young",
    "email": "youngmd@iu.edu",
    "headshot": "5d9b7fcc557d063fe591fdfb",
    "__v": 0,
    "joined": "2012-05-14T00:00:00.000Z",
    "background": "Ph.D in Astronomy (IU 2016)",
    "sca": true,
    "uid": "youngmd",
    "view_rank": 2
  }, {
    "active": true,
    "_id": "5d9cc2c1cb13e070e2513950",
    "name": "Scott Michael",
    "email": "scamicha@iu.edu",
    "role": "Director, Research and Software Solutions",
    "background": "Scott took over as director of Research and Software Solutions within Research Technologies in Oct 2021. Previously, Scott was a key collaborator as the manager of the Research Applications and Deep Learning (RADL) team at IU.",
    "joined": null,
    "sca": false,
    "view_rank": 8,
    "headshot": "5d9cc2c1cb13e070e251394e",
    "__v": 0,
    "uid": "scamicha"
  }],
  "_id": "5dc5938548fbdd548b2d42df",
  "bib_string": "Young, M. D., Michael, S. 2017.  Big Data Challenges in the Blanco DECam Bulge Survey.  Astronomical Data Analysis Software and Systems XXV, Volume 512 (December 2017);",
  "date": null,
  "doi": "",
  "links": [{
    "_id": "5dc5938548fbdd548b2d42e0",
    "url": "http://aspbooks.org/publications/512/189.pdf",
    "label": "Full Paper (PDF)"
  }, {
    "_id": "60df72f068220235caa2521d",
    "url": "https://drive.google.com/file/d/1R0ZBFFbs6VbzujGdkLRMrrkDNn1PSRKB/view?usp=sharing",
    "label": "Conference Poster (PDF)"
  }],
  "__v": 2
}])

const first_author = computed(() => {
  if(props.showAll) return papers.value
  let first = papers.value.filter(p => {
    return p.bib_string.startsWith('Young')
  })
  return first.slice(0, 5)
})

</script>


<template>
  <li v-for="p in first_author" class="lg:text-lg text list-none mb-2">
    {{ p.bib_string }}
    <div class="text-sm font-light ml-5">
      <span v-for="l in p.links"> | <a :href="l.url" target="_blank">{{l.label}} </a> </span>
    </div>
  </li>
</template>
