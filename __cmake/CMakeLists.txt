LINK_DIRECTORIES(${CMAKE_ARCHIVE_OUTPUT_DIRECTORY})
add_subdirectory(TimDemo)
add_subdirectory(UiEditor)
add_subdirectory(qqlogin)
add_subdirectory(360)
add_subdirectory(360Preview)
add_subdirectory(souispy)
add_subdirectory(PcManager)
add_subdirectory(SoTool)
add_subdirectory(mclistview_demo)
add_subdirectory(souitest)
add_subdirectory(VUI)
add_subdirectory(BesLyric)
add_subdirectory(QQMain)
add_subdirectory(FrogPlay)
add_subdirectory(MultiLangs)
add_subdirectory(TXMgr)
add_subdirectory(SLogViewer)
add_subdirectory(souieditor)
add_subdirectory(DropDemo)
add_subdirectory(ThreeClearGame)
add_subdirectory(baiduwp)
add_subdirectory(ScreenShotTool)
add_subdirectory(SoftMaster)
add_subdirectory(SweepingEdge)
add_subdirectory(iectrl)
add_subdirectory(mfc.demo)
add_subdirectory(CapScreenDemo)
#add_subdirectory(SOUI-CEF)
#add_subdirectory(nsisdemo/setupdll)
add_subdirectory(SouiWallPaper)
add_subdirectory(TczKline)
add_subdirectory(SIpcDemo)

include(CheckCXXCompilerFlag)
CHECK_CXX_COMPILER_FLAG("-std=c++11" COMPILER_SUPPORTS_CXX11)
if(COMPILER_SUPPORTS_CXX11)
	add_subdirectory(TIMDemo)
	message(STATUS "build TIMDemo ON")
else()
	message(STATUS "build TIMDemo OFF")
endif()
