<template>
  <div class="container mx-auto mt-[10rem]">
    <h1 class="title-font text-center text-5xl py-5 ">
      电子书和试卷
    </h1>
    <ClientOnly>
      <Suspense>
        <ListProvider />
        <template #fallback>
          <div class="flex justify-center h-50 items-center">
            <TLoading size="large" />
          </div>
        </template>
      </Suspense>
    </ClientOnly>
  </div>
</template>
