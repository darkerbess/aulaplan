<script>
  import { Container, TabContent, TabPane } from "sveltestrap";
  import Calendar from "@event-calendar/core";
  import DayGrid from "@event-calendar/day-grid";

  let plugins = [DayGrid];
  let options = {
    firstDay: 1,
    height: "auto",
    view: "dayGridMonth",
    events: [{ month: "Feb", day: "21", year: "2022" }],
  };
</script>

<div style="background-color: #FEFEFE;" class="pt-4">
  <Container>
    <TabContent>
      <TabPane tabId="calendar" tab="Calendar" active class="my-3">
        <Calendar {plugins} {options} />
      </TabPane>
      <TabPane tabId="tasks" tab="Tasks" class="my-3">
        <h2>Tasks</h2>
      </TabPane>
      <TabPane tabId="schedule" tab="Schedule" class="my-3">
        <Calendar {plugins} {options} />
      </TabPane>
    </TabContent>
  </Container>
</div>
