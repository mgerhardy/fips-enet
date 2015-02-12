fips_begin_lib(enet)
	include_directories(enet)
	fips_files(
	)
	# hack to silence some warnings
	#if (FIPS_MACOS)
	#	set_target_properties(enet PROPERTIES COMPILE_FLAGS "-Wno-sign-compare -Wno-deprecated-declarations")
	#elseif(FIPS_LINUX)
	#	set_target_properties(enet PROPERTIES COMPILE_FLAGS "-Wno-sign-compare")
	#endif()
fips_end_lib()
