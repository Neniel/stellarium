
########### install files ###############

# install info.ini
INSTALL(FILES info.ini DESTINATION ${SDATALOC}/skycultures/greek_almagest )

# install constellations data, native names data, artwork and descriptions
INSTALL(DIRECTORY ./ DESTINATION ${SDATALOC}/skycultures/greek_almagest
	FILES_MATCHING PATTERN "*.fab" 
	PATTERN "*.utf8"
	PATTERN "*.png"
	PATTERN "CMakeFiles" EXCLUDE )
