TOP=..
include $(TOP)/configure/CONFIG
#=======================================

DB += devKeithley6482.db
DB += $(TOP)/Keithley6482Sup/devKeithley6482.proto

# Install .dbd and .db files
DB_INSTALLS += devKeithley6482.db
DB_INSTALLS += zeroCorrect.db
DB_INSTALLS += $(TOP)/Keithley6482Sup/devKeithley6482.proto
ifdef AUTOSAVE_ASSUPPORT
IOCManager_DBD += asSupport.dbd
else 
IOCManager_DBD +=autosaveSupport.db
endif

#DB_INSTALLS += $(...)/db/save_restoreStatus.db

# Install library
ifdef RESTORE
IOCManager_LIBS += restore
endif
IOCManager_LIBS += autosave

#=======================================
include $(TOP)/configure/RULES
