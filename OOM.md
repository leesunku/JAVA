 #OOM(E) - Out Of Memory Error는 JVM이 일정한 크기의 메모리를 할당하는데 실패하면 발생합니다. 원인은 다양한데,
 ###Java Heap : Java Heap Space의 부족으로 Object를 생성하지 못한 경우나, Java Heap의 최대 크기보다 큰 Array가 요청되는 경우입니다.
 ###Memory Leak : 대부분 잘못된 Application 로직에 의해 발생, Object에 대한 참조(Reference)관계가 복잡한 경우등에 Garbage Collection에 의해 메모리 해제가 이루어지지 않아 발생합니다.
 ###Native Heap : Native Heap은 OS 레벨의 Native Object가 거주하는 공간입니다. VM code 레벨에서 메모리 부족 현상이 발견되거나, Thread를 생성할 수 없을 때 발생합니다. Thread는 Native Heap 공간의 메모리를 필요로 하기 때문에 Native Heap 공간의 메모리가 부족하면 발생합니다.
 
