# $FreeBSD$

.include <bsd.own.mk>
.include "Makefile.inc"

SUBDIR=		dtmalloc	\
		dtnfscl		\
		dtnfsclient	\
		dtrace		\
		dtraceall	\
		dtrace_test	\
		dtio		\
		prototype	\
		sdt		\
		systrace

.if ${MACHINE_CPUARCH} == "amd64" || ${MACHINE_CPUARCH} == "i386"
SUBDIR+=	fasttrap fbt lockstat profile systrace_linux32
.endif
.if ${MACHINE_CPUARCH} == "amd64"
SUBDIR+=	systrace_freebsd32
.endif

.include <bsd.subdir.mk>
