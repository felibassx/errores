# Errores con los paquetes de firebase 

Plugin project :firebase_core_web not found. Please update settings.gradle.
Plugin project :firebase_auth_web not found. Please update settings.gradle.
Plugin project :cloud_firestore_web not found. Please update settings.gradle.
Note: /Users/kafecode/.pub-cache/hosted/pub.dartlang.org/cloud_firestore-0.13.6/android/src/main/java/io/flutter/plugins/firebase/cloudfirestore/CloudFirestorePlugin.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
D8: Cannot fit requested classes in a single dex file (# methods: 81769 > 65536)
com.android.builder.dexing.DexArchiveMergerException: Error while merging dex archives: 
The number of method references in a .dex file cannot exceed 64K.
Learn how to resolve this issue at https://developer.android.com/tools/building/multidex.html
	at com.android.builder.dexing.D8DexArchiveMerger.getExceptionToRethrow(D8DexArchiveMerger.java:131)
	at com.android.builder.dexing.D8DexArchiveMerger.mergeDexArchives(D8DexArchiveMerger.java:118)
	at com.android.build.gradle.internal.transforms.DexMergerTransformCallable.call(DexMergerTransformCallable.java:102)
	at com.android.build.gradle.internal.tasks.DexMergingTaskRunnable.run(DexMergingTask.kt:444)
	at com.android.build.gradle.internal.tasks.Workers$ActionFacade.run(Workers.kt:335)
	at org.gradle.workers.internal.AdapterWorkAction.execute(AdapterWorkAction.java:50)
	at org.gradle.workers.internal.DefaultWorkerServer.execute(DefaultWorkerServer.java:47)
	at org.gradle.workers.internal.NoIsolationWorkerFactory$1$1$1.create(NoIsolationWorkerFactory.java:65)
	at org.gradle.workers.internal.NoIsolationWorkerFactory$1$1$1.create(NoIsolationWorkerFactory.java:61)
	at org.gradle.internal.classloader.ClassLoaderUtils.executeInClassloader(ClassLoaderUtils.java:98)
	at org.gradle.workers.internal.NoIsolationWorkerFactory$1$1.execute(NoIsolationWorkerFactory.java:61)
	at org.gradle.workers.internal.AbstractWorker$1.call(AbstractWorker.java:44)
	at org.gradle.workers.internal.AbstractWorker$1.call(AbstractWorker.java:41)
	at org.gradle.internal.operations.DefaultBuildOperationExecutor$CallableBuildOperationWorker.execute(DefaultBuildOperationExecutor.java:416)
	at org.gradle.internal.operations.DefaultBuildOperationExecutor$CallableBuildOperationWorker.execute(DefaultBuildOperationExecutor.java:406)
	at org.gradle.internal.operations.DefaultBuildOperationExecutor$1.execute(DefaultBuildOperationExecutor.java:165)
	at org.gradle.internal.operations.DefaultBuildOperationExecutor.execute(DefaultBuildOperationExecutor.java:250)
	at org.gradle.internal.operations.DefaultBuildOperationExecutor.execute(DefaultBuildOperationExecutor.java:158)
	at org.gradle.internal.operations.DefaultBuildOperationExecutor.call(DefaultBuildOperationExecutor.java:102)
	at org.gradle.internal.operations.DelegatingBuildOperationExecutor.call(DelegatingBuildOperationExecutor.java:36)
	at org.gradle.workers.internal.AbstractWorker.executeWrappedInBuildOperation(AbstractWorker.java:41)
	at org.gradle.workers.internal.NoIsolationWorkerFactory$1.execute(NoIsolationWorkerFactory.java:56)
	at org.gradle.workers.internal.DefaultWorkerExecutor$3.call(DefaultWorkerExecutor.java:215)
	at org.gradle.workers.internal.DefaultWorkerExecutor$3.call(DefaultWorkerExecutor.java:210)
	at java.util.concurrent.FutureTask.run(FutureTask.java:266)
	at org.gradle.internal.work.DefaultConditionalExecutionQueue$ExecutionRunner.runExecution(DefaultConditionalExecutionQueue.java:215)
	at org.gradle.internal.work.DefaultConditionalExecutionQueue$ExecutionRunner.runBatch(DefaultConditionalExecutionQueue.java:164)
	at org.gradle.internal.work.DefaultConditionalExecutionQueue$ExecutionRunner.run(DefaultConditionalExecutionQueue.java:131)
	at java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:511)
	at java.util.concurrent.FutureTask.run(FutureTask.java:266)
	at org.gradle.internal.concurrent.ExecutorPolicy$CatchAndRecordFailures.onExecute(ExecutorPolicy.java:64)
	at org.gradle.internal.concurrent.ManagedExecutorImpl$1.run(ManagedExecutorImpl.java:48)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624)
	at org.gradle.internal.concurrent.ThreadFactoryImpl$ManagedThreadRunnable.run(ThreadFactoryImpl.java:56)
	at java.lang.Thread.run(Thread.java:748)
Caused by: com.android.tools.r8.CompilationFailedException: Compilation failed to complete
	at com.android.tools.r8.utils.t.a(:55)
	at com.android.tools.r8.D8.run(:11)
	at com.android.builder.dexing.D8DexArchiveMerger.mergeDexArchives(D8DexArchiveMerger.java:116)
	... 34 more
Caused by: com.android.tools.r8.utils.AbortException: Error: null, Cannot fit requested classes in a single dex file (# methods: 81769 > 65536)
	at com.android.tools.r8.utils.Reporter.a(:21)
	at com.android.tools.r8.utils.Reporter.a(:7)
	at com.android.tools.r8.dex.VirtualFile.a(:33)
	at com.android.tools.r8.dex.VirtualFile$h.a(:5)
	at com.android.tools.r8.dex.ApplicationWriter.a(:13)
	at com.android.tools.r8.dex.ApplicationWriter.write(:35)
	at com.android.tools.r8.D8.d(:44)
	at com.android.tools.r8.D8.b(:1)
	at com.android.tools.r8.utils.t.a(:23)
	... 36 more

FAILURE: Build failed with an exception.
* What went wrong:
Execution failed for task ':app:mergeDexDebug'.
> A failure occurred while executing com.android.build.gradle.internal.tasks.Workers$ActionFacade
   > com.android.builder.dexing.DexArchiveMergerException: Error while merging dex archives: 
     The number of method references in a .dex file cannot exceed 64K.
     Learn how to resolve this issue at https://developer.android.com/tools/building/multidex.html

* Try:
Run with --stacktrace option to get the stack trace. Run with --info or --debug option to get more log output. Run with --scan to get full insights.

* Get more help at https://help.gradle.org

BUILD FAILED in 39s
[!] The shrinker may have failed to optimize the Java bytecode.
    To disable the shrinker, pass the `--no-shrink` flag to this command.
    To learn more, see: https://developer.android.com/studio/build/shrink-code
Exception: Gradle task assembleDebug failed with exit code 1
Exited (sigterm)
