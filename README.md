import { Card, CardContent } from "@/components/ui/card";
import { Tabs, TabsList, TabsTrigger, TabsContent } from "@/components/ui/tabs";
import { Button } from "@/components/ui/button";
import { CalendarDays, FileText, LayoutDashboard, Users, Mail } from "lucide-react";

export default function ProjectTemplatePage() {
  return (
    <div className="p-6 space-y-6">
      <h1 className="text-3xl font-bold text-center">Tesla Dynamic and Smart Manufacturing Inc.</h1>
      <p className="text-center text-muted-foreground">Website Project Template</p>

      <Tabs defaultValue="overview" className="mt-6">
        <TabsList className="grid w-full grid-cols-6">
          <TabsTrigger value="overview">Overview</TabsTrigger>
          <TabsTrigger value="scope">Scope</TabsTrigger>
          <TabsTrigger value="timeline">Timeline</TabsTrigger>
          <TabsTrigger value="admin">Admin Dashboard</TabsTrigger>
          <TabsTrigger value="team">Team</TabsTrigger>
          <TabsTrigger value="contact">Contact</TabsTrigger>
        </TabsList>

        <TabsContent value="overview">
          <Card>
            <CardContent className="p-6 space-y-4">
              <h2 className="text-xl font-semibold">Project Overview</h2>
              <p>This project is aimed at designing and developing a modern, responsive website for Tesla Dynamic and Smart Manufacturing Inc. The new platform will serve as a central hub to showcase our advanced manufacturing capabilities, innovative solutions, and corporate values.</p>

              <h3 className="text-lg font-medium">Objectives</h3>
              <ul className="list-disc pl-6 space-y-1">
                <li>Create a professional, high-performing website.</li>
                <li>Ensure responsiveness across all devices.</li>
                <li>Optimize for SEO and search engine ranking.</li>
                <li>Integrate contact forms and lead capture.</li>
                <li>Provide an easy-to-use CMS.</li>
              </ul>
            </CardContent>
          </Card>
        </TabsContent>

        <TabsContent value="scope">
          <Card>
            <CardContent className="p-6 space-y-4">
              <h2 className="text-xl font-semibold">Scope of Work</h2>
              <ul className="list-disc pl-6 space-y-1">
                <li>Custom UI/UX Design</li>
                <li>Frontend & Backend Development</li>
                <li>SEO and Performance Optimization</li>
                <li>CMS Integration</li>
                <li>Testing and Deployment</li>
              </ul>

              <h3 className="text-lg font-medium mt-4">Roles & Responsibilities</h3>
              <ul className="list-disc pl-6 space-y-1">
                <li>Project Lead – Oversees full project lifecycle</li>
                <li>Designer – Creates UI/UX mockups</li>
                <li>Developer – Builds and integrates site features</li>
                <li>QA Specialist – Conducts thorough testing</li>
              </ul>
            </CardContent>
          </Card>
        </TabsContent>

        <TabsContent value="timeline">
          <Card>
            <CardContent className="p-6 space-y-4">
              <h2 className="text-xl font-semibold">Project Timeline</h2>
              <div className="space-y-2">
                <div className="flex justify-between">
                  <span>Discovery & Planning</span>
                  <span>[Insert Dates]</span>
                </div>
                <div className="flex justify-between">
                  <span>Design Phase</span>
                  <span>[Insert Dates]</span>
                </div>
                <div className="flex justify-between">
                  <span>Development Phase</span>
                  <span>[Insert Dates]</span>
                </div>
                <div className="flex justify-between">
                  <span>Testing</span>
                  <span>[Insert Dates]</span>
                </div>
                <div className="flex justify-between">
                  <span>Launch</span>
                  <span>[Insert Dates]</span>
                </div>
              </div>
            </CardContent>
          </Card>
        </TabsContent>

        <TabsContent value="admin">
          <Card>
            <CardContent className="p-6 space-y-4">
              <h2 className="text-xl font-semibold flex items-center gap-2"><LayoutDashboard /> Admin Dashboard</h2>
              <p>Manage content, monitor site performance, and assign roles.</p>
              <ul className="list-disc pl-6 space-y-1">
                <li>Content Management (pages, media, blog)</li>
                <li>User Role Assignment (Admin, Editor, Viewer)</li>
                <li>Site Analytics Overview</li>
                <li>SEO and Performance Tools Access</li>
              </ul>
              <Button className="mt-4">Go to Admin Panel</Button>
            </CardContent>
          </Card>
        </TabsContent>

        <TabsContent value="team">
          <Card>
            <CardContent className="p-6 space-y-4">
              <h2 className="text-xl font-semibold flex items-center gap-2"><Users /> Meet the Team</h2>
              <p>Our dedicated team of professionals ensures success in every project phase.</p>
              <ul className="list-disc pl-6 space-y-1">
                <li>John Doe – CEO & Founder</li>
                <li>Jane Smith – Lead Developer</li>
                <li>Michael Brown – UX/UI Designer</li>
                <li>Sarah Wilson – QA Specialist</li>
              </ul>
            </CardContent>
          </Card>
        </TabsContent>

        <TabsContent value="contact">
          <Card>
            <CardContent className="p-6 space-y-4">
              <h2 className="text-xl font-semibold flex items-center gap-2"><Mail /> Contact Us</h2>
              <p>We would love to hear from you. Please use the form below to get in touch.</p>
              <form className="space-y-4">
                <div>
                  <label className="block text-sm font-medium">Name</label>
                  <input type="text" className="w-full border rounded p-2" placeholder="Your name" />
                </div>
                <div>
                  <label className="block text-sm font-medium">Email</label>
                  <input type="email" className="w-full border rounded p-2" placeholder="Your email" />
                </div>
                <div>
                  <label className="block text-sm font-medium">Message</label>
                  <textarea className="w-full border rounded p-2" rows={4} placeholder="Your message"></textarea>
                </div>
                <Button type="submit">Send Message</Button>
              </form>
            </CardContent>
          </Card>
        </TabsContent>
      </Tabs>
    </div>
  );
}
