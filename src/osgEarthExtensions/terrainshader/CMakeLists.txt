#
# terrain shader plugin
#
set(TARGET_SRC
	TerrainShaderPlugin.cpp
	TerrainShaderExtension.cpp
	${SHADERS_CPP} )
	
set(LIB_PUBLIC_HEADERS
	TerrainShaderExtension
	TerrainShaderOptions)
	
set(TARGET_H
	${LIB_PUBLIC_HEADERS})


set(TARGET_COMMON_LIBRARIES ${TARGET_COMMON_LIBRARIES}
    osgEarthUtil)
	
setup_extension(osgearth_terrainshader)

# to install public driver includes:
set(LIB_NAME terrainshader)

