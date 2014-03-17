include Common/CommonDefs.mak

.PHONY: all

NETPROJ = 
ifneq "$(realpath /usr/bin/gmcs)" ""
endif

all: $(NETPROJ) SimpleRead.java NiSimpleRead NiConvertXToONI NiSimpleSkeleton NiSampleModule NiRecordSynthetic NiCRead NiAudioSample NiSimpleCreate NiSkeletonBenchmark UserTracker.java NiBackRecorder SimpleViewer.java 


.PHONY: SimpleRead.java
SimpleRead.java:
	$(MAKE) -C ../SimpleRead.java

.PHONY: NiSimpleRead
NiSimpleRead:
	$(MAKE) -C ../NiSimpleRead

.PHONY: NiConvertXToONI
NiConvertXToONI:
	$(MAKE) -C ../NiConvertXToONI

.PHONY: NiSimpleSkeleton
NiSimpleSkeleton:
	$(MAKE) -C ../NiSimpleSkeleton

.PHONY: NiSampleModule
NiSampleModule:
	$(MAKE) -C ../NiSampleModule

.PHONY: NiRecordSynthetic
NiRecordSynthetic:
	$(MAKE) -C ../NiRecordSynthetic

.PHONY: NiCRead
NiCRead:
	$(MAKE) -C ../NiCRead

.PHONY: NiAudioSample
NiAudioSample:
	$(MAKE) -C ../NiAudioSample

.PHONY: NiSimpleCreate
NiSimpleCreate:
	$(MAKE) -C ../NiSimpleCreate

.PHONY: NiSkeletonBenchmark
NiSkeletonBenchmark:
	$(MAKE) -C ../NiSkeletonBenchmark

.PHONY: UserTracker.java
UserTracker.java:
	$(MAKE) -C ../UserTracker.java

.PHONY: NiBackRecorder
NiBackRecorder:
	$(MAKE) -C ../NiBackRecorder

.PHONY: SimpleViewer.java
SimpleViewer.java:
	$(MAKE) -C ../SimpleViewer.java
