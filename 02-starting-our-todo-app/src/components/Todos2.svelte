<!-- Todos.svelte -->
<div class="todoapp stack-large">
  <!-- 새로운 할일 -->
  <form>
    <h2 class="label-wrapper">
      <label for="todo-0" class="label__lg"> 무엇을 해야하나요? </label>
    </h2>
    <input type="text" id="todo-0" autocomplete="off" class="input input__lg" />
    <button type="submit" disabled="" class="btn btn__primary btn__lg">
      추가
    </button>
  </form>

  <!-- 필터 -->
  <div class="filters btn-group stack-exception">
    <button class="btn toggle-btn" aria-pressed="true">
      <span class="visually-hidden">나타내기</span>
      <span>모두 보기</span>
      <span class="visually-hidden">작업</span>
    </button>
    <button class="btn toggle-btn" aria-pressed="false">
      <span class="visually-hidden">나타내기</span>
      <span>활성화</span>
      <span class="visually-hidden">작업</span>
    </button>
    <button class="btn toggle-btn" aria-pressed="false">
      <span class="visually-hidden">나타내기</span>
      <span>완료</span>
      <span class="visually-hidden">작업</span>
    </button>
  </div>

  <!-- 할 일 상태 -->
  <h2 id="list-heading">3개 항목 중 2개 완료</h2>

  <!-- 할 일들 -->
  <ul role="list" class="todo-list stack-large" aria-labelledby="list-heading">
    <!-- 할 일 1 (수정 모드) -->
    <li class="todo">
      <div class="stack-small">
        <form class="stack-small">
          <div class="form-group">
            <label for="todo-1" class="todo-label">
              'Svelte 시작 앱 만들기'의 새 이름
            </label>
            <input
              type="text"
              id="todo-1"
              autocomplete="off"
              class="todo-text" />
          </div>
          <div class="btn-group">
            <button class="btn todo-cancel" type="button">
              취소
              <span class="visually-hidden">Svelte 스타터 앱 만들기</span>
            </button>
            <button class="btn btn__primary todo-edit" type="submit">
              저장
              <span class="visually-hidden">Svelte 스타터 앱 만들기의 새 이름</span>
            </button>
          </div>
        </form>
      </div>
    </li>

    <!-- 할 일 2 -->
    <li class="todo">
      <div class="stack-small">
        <div class="c-cb">
          <input type="checkbox" id="todo-2" checked />
          <label for="todo-2" class="todo-label">
            첫 번째 컴포넌트 생성
          </label>
        </div>
        <div class="btn-group">
          <button type="button" class="btn">
            수정
            <span class="visually-hidden">첫 번째 새로운 컴포넌트 생성</span>
          </button>
          <button type="button" class="btn btn__danger">
            삭제
            <span class="visually-hidden">첫 번째 새로운 컴포넌트 생성</span>
          </button>
        </div>
      </div>
    </li>

    <!-- 할 일 3 -->
    <li class="todo">
      <div class="stack-small">
        <div class="c-cb">
          <input type="checkbox" id="todo-3" />
          <label for="todo-3" class="todo-label">
            나머지 튜토리얼 완료
          </label>
        </div>
        <div class="btn-group">
          <button type="button" class="btn">
            수정
            <span class="visually-hidden">나머지 튜토리얼 완료</span>
          </button>
          <button type="button" class="btn btn__danger">
            삭제
            <span class="visually-hidden">나머지 튜토리얼 완료</span>
          </button>
        </div>
      </div>
    </li>
  </ul>

  <hr />

  <!-- 다른 액션 -->
  <div class="btn-group">
    <button type="button" class="btn btn__primary">모두 체크</button>
    <button type="button" class="btn btn__primary">완전히 삭제</button>
  </div>
</div>

